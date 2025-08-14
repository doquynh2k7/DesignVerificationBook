.. _cong_cu_thiet_ke:

===================
doxygen
===================

``doxygen`` is the core integration-level module for mqnic for the PCIe host interface.  Wrapper around, adding PCIe DMA interface module and PCIe-AXI Lite masters for the NIC and application control BARs.

This module implements a generic PCIe host interface, which must be adapted to the target device with a wrapper.  The available wrappers are:

