---
title: '방법: 클릭한 TreeView 노드 확인(Windows Forms)'
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
- cpp
f1_keywords:
- TreeNode
helpviewer_keywords:
- examples [Windows Forms], TreeView control
- tree nodes in TreeView control [Windows Forms], determining node clicked
- TreeView control [Windows Forms], determining node clicked
ms.assetid: 06a4a191-d918-42af-9f49-956c93eff261
ms.openlocfilehash: d1e9df6a928f1ea60e4663c78d204ec2b16baf23
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
ms.locfileid: "33530629"
---
# <a name="how-to-determine-which-treeview-node-was-clicked-windows-forms"></a>방법: 클릭한 TreeView 노드 확인(Windows Forms)
Windows Forms 작업할 때 <xref:System.Windows.Forms.TreeView> 컨트롤은 일반적인 작업 결정 하는 것 노드 클릭 되었는지와 적절 하 게 응답 합니다.  
  
### <a name="to-determine-which-treeview-node-was-clicked"></a>클릭 한 TreeView 노드 확인  
  
1.  사용 하 여는 <xref:System.EventArgs> 클릭 한 노드 개체에 대 한 참조를 반환 하는 개체입니다.  
  
2.  노드를 선택 하 여 클릭 했는지 확인는 <xref:System.Windows.Forms.TreeViewEventArgs> 이벤트와 관련 된 데이터를 포함 하는 클래스입니다.  
  
    ```vb  
    Private Sub TreeView1_AfterSelect(ByVal sender As System.Object, _  
    ByVal e As System.Windows.Forms.TreeViewEventArgs) Handles TreeView1.AfterSelect  
       ' Determine by checking the Node property of the TreeViewEventArgs.  
       MessageBox.Show(e.Node.Text)  
    End Sub  
    ```  
  
    ```csharp  
    protected void treeView1_AfterSelect (object sender,   
    System.Windows.Forms.TreeViewEventArgs e)  
    {  
       // Determine by checking the Text property.  
       MessageBox.Show(e.Node.Text);  
    }  
    ```  
  
    ```cpp  
    private:  
       void treeView1_AfterSelect(System::Object ^  sender,  
          System::Windows::Forms::TreeViewEventArgs ^  e)  
       {  
          // Determine by checking the Text property.  
          MessageBox::Show(e->Node->Text);  
       }  
    ```  
  
    > [!NOTE]
    >  사용할 수 있습니다는 <xref:System.Windows.Forms.MouseEventArgs> 의 <xref:System.Windows.Forms.Control.MouseDown> 또는 <xref:System.Windows.Forms.Control.MouseUp> 가져올 이벤트는 <xref:System.Drawing.Point.X%2A> 및 <xref:System.Drawing.Point.Y%2A> 좌표 값은 <xref:System.Drawing.Point> 클릭이 발생 합니다. 다음을 사용 하 여는 <xref:System.Windows.Forms.TreeView> 컨트롤의 <xref:System.Windows.Forms.TreeView.GetNodeAt%2A> 클릭 된 노드를 확인할 수 있습니다.  
  
## <a name="see-also"></a>참고 항목  
 [TreeView 컨트롤](../../../../docs/framework/winforms/controls/treeview-control-windows-forms.md)
