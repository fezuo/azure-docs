---
title: 'Copy and paste to and from a Windows virtual machine: Azure Bastion'
description: Learn how copy and paste to and from a Windows VM using Bastion.
services: bastion
author: cherylmc

ms.service: bastion
ms.topic: how-to
ms.date: 08/30/2021
ms.author: cherylmc
# Customer intent: I want to copy and paste to and from VMs using Azure Bastion.

---

# Copy and paste to a Windows virtual machine: Azure Bastion

This article helps you copy and paste text to and from virtual machines when using Azure Bastion. Before you work with a VM, make sure you have followed the steps to [Create a Bastion host](./tutorial-create-host-portal.md). Then, connect to the VM that you want to work with using either [RDP](bastion-connect-vm-rdp-windows.md) or [SSH](bastion-connect-vm-ssh-windows.md).

For browsers that support the advanced Clipboard API access, you can copy and paste text between your local device and the remote session in the same way you copy and paste between applications on your local device. For other browsers, you can use the Bastion clipboard access tool palette.

>[!NOTE]
>Only text copy/paste is currently supported.
>

   ![Allow clipboard](./media/bastion-vm-manage/allow.png)

Only text copy/paste is supported. For direct copy and paste, your browser may prompt you for clipboard access when the Bastion session is being initialized. **Allow** the web page to access the clipboard. If you are working from a Mac, the keyboard shortcut to paste is **SHIFT-CTRL-V**.

## <a name="to"></a>Copy to a remote session

After you connect to the virtual machine using the [Azure portal ](https://portal.azure.com), complete the following steps:

1. Copy the text/content from the local device into local clipboard.
1. During the remote session, launch the Bastion clipboard access tool palette by selecting the two arrows. The arrows are located on the left center of the session.

   ![Screenshot that shows the launch arrows for the tool palette highlighted on the left-side of the window.](./media/bastion-vm-manage/left.png)

   ![Screenshot shows a clipboard for text copied in Bastion.](./media/bastion-vm-manage/clipboard.png)
1. Typically, the copied text automatically shows on the Bastion copy paste palette. If your text is not there, then paste the text in the text area on the palette.
1. Once the text is in the text area, you can paste it to the remote session.

   ![Screenshot that shows the copy/paste button highlighted and a sample text string copied into the remote session.](./media/bastion-vm-manage/local.png)

## <a name="from"></a>Copy from a remote session

After you connect to the virtual machine using the [Azure portal ](https://portal.azure.com), complete the following steps:

1. Copy the text/content from the remote session into remote clipboard (using Ctrl-C).

   ![tool palette](./media/bastion-vm-manage/remote.png)
1. During the remote session, launch the Bastion clipboard access tool palette by selecting the two arrows. The arrows are located on the left center of the session.

   ![clipboard](./media/bastion-vm-manage/clipboard2.png)
1. Typically, the copied text automatically shows on the Bastion copy paste palette. If your text is not there, then paste the text in the text area on the palette.
1. Once the text is in the text area, you can paste it to the local device.

   ![paste](./media/bastion-vm-manage/local2.png)
 
## Next steps

Read the [Bastion FAQ](bastion-faq.md).
