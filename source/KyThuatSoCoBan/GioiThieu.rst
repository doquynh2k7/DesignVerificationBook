.. _KyThuatSoCoBan_GioiThieu:

==========
Giới Thiệu
==========

Giới thiệu cho kỹ thuật số cơ bản


Qui trình cho một thiết kế
==========================

.. _fig_overview_block:
.. figure:: https://1.bp.blogspot.com/-qIReehJ0Hro/XrROQDYUmFI/AAAAAAAAaGw/LUeiaa4Ic44TfQ1ZmdLIz4-agwaCLIsMACK4BGAsYHg/w640-h627/asic_flow1.png

    Block diagram of the Corundum NIC. PCIe HIP: PCIe hard IP core; AXIL M: AXI lite master; DMA IF: DMA interface; AXI M: AXI master; PHC: PTP hardware clock; TXQ: transmit queue manager; TXCQ: transmit completion queue manager; RXQ: receive queue manager; RXCQ: receive completion queue manager; EQ: event queue manager; MAC + PHY: Ethernet media access controller (MAC) and physical interface layer (PHY).

A  block diagram of the Corundum NIC is shown in :numref:`fig_overview_block`.  At a high level, the NIC consists of several hierarchy levels.  The top-level module primarily contains support and interfacing components. These components include the PCI express hard IP core and Ethernet interface components including MACs, PHYs, and associated serializers, along with an instance of an appropriate :ref:`mod_mqnic_core` wrapper, which provides the DMA interface.