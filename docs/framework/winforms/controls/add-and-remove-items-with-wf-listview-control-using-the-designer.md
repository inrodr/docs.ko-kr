---
title: '방법: 디자이너를 사용하여 Windows Forms ListView 컨트롤에서 항목 추가 및 제거'
ms.date: 03/30/2017
helpviewer_keywords:
- ListView control [Windows Forms], populating
- ListView control [Windows Forms], adding list items
ms.assetid: 217611ee-fd11-4d39-9a54-a37c3e781be1
ms.openlocfilehash: 0480c8980f0eba17229fff0c1e947cac5216fb9e
ms.sourcegitcommit: 8c28ab17c26bf08abbd004cc37651985c68841b8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/07/2018
ms.locfileid: "48847752"
---
# <a name="how-to-add-and-remove-items-with-the-windows-forms-listview-control-using-the-designer"></a>방법: 디자이너를 사용하여 Windows Forms ListView 컨트롤에서 항목 추가 및 제거
Windows Forms에 항목을 추가 하는 프로세스 <xref:System.Windows.Forms.ListView> 컨트롤 주로 이루어져 항목을 지정 하 고 속성을 할당 합니다. 목록 항목 추가 또는 제거를 언제 든 지 수행할 수 있습니다.  
  
 다음 절차를 수행 하려면을 **Windows 응용 프로그램** 포함 하는 양식을 사용 하 여 프로젝트를 <xref:System.Windows.Forms.ListView> 제어 합니다. 이러한 프로젝트 설정에 대 한 자세한 내용은 [방법: Windows 응용 프로그램 프로젝트를 만듭니다](https://msdn.microsoft.com/library/b2f93fed-c635-4705-8d0e-cf079a264efa) 및 [방법: Windows Forms에 컨트롤 추가](../../../../docs/framework/winforms/controls/how-to-add-controls-to-windows-forms.md)합니다.  
  
> [!NOTE]
>  표시되는 대화 상자와 메뉴 명령은 활성 설정이나 버전에 따라 도움말에서 설명하는 것과 다를 수 있습니다. 설정을 변경하려면 **도구** 메뉴에서 **설정 가져오기 및 내보내기** 를 선택합니다. 자세한 내용은 [Visual Studio IDE 개인 설정](/visualstudio/ide/personalizing-the-visual-studio-ide)을 참조하세요.  
  
### <a name="to-add-or-remove-items-using-the-designer"></a>디자이너를 사용 하 여 항목을 추가 하거나 제거  
  
1.  <xref:System.Windows.Forms.ListView> 컨트롤을 선택합니다.  
  
2.  에 **속성** 창에서 클릭 합니다 **줄임표** (![VisualStudioEllipsesButton 스크린 샷](../../../../docs/framework/winforms/media/vbellipsesbutton.png "vbEllipsesButton")) 단추 옆에 <xref:System.Windows.Forms.ListView.Items%2A> 속성입니다.  
  
     합니다 **ListViewItem 컬렉션 편집기** 나타납니다.  
  
3.  항목을 추가 하려면 클릭 합니다 **추가** 단추입니다. 새 항목의 속성을 같은 설정한 수는 <xref:System.Windows.Forms.ListView.Text%2A> 고 <xref:System.Windows.Forms.ListViewItem.ImageIndex%2A> 속성입니다.  
  
4.  항목을 제거 하려면 선택 하 고 클릭 합니다 **제거** 단추입니다.  
  
## <a name="see-also"></a>참고 항목  
 [ListView 컨트롤 개요](../../../../docs/framework/winforms/controls/listview-control-overview-windows-forms.md)  
 [방법: Windows Forms ListView 컨트롤에 열 추가](../../../../docs/framework/winforms/controls/how-to-add-columns-to-the-windows-forms-listview-control.md)  
 [방법: Windows Forms ListView 컨트롤을 사용하여 열에 하위 항목 표시](../../../../docs/framework/winforms/controls/how-to-display-subitems-in-columns-with-the-windows-forms-listview-control.md)  
 [방법: Windows Forms ListView 컨트롤의 아이콘 표시](../../../../docs/framework/winforms/controls/how-to-display-icons-for-the-windows-forms-listview-control.md)  
 [방법: TreeView 또는 ListView 컨트롤에 사용자 지정 정보 추가(Windows Forms)](../../../../docs/framework/winforms/controls/add-custom-information-to-a-treeview-or-listview-control-wf.md)  
 [방법: Windows Forms ListView 컨트롤에서 항목 그룹화](../../../../docs/framework/winforms/controls/how-to-group-items-in-a-windows-forms-listview-control.md)
