---
title: '방법: 시스템 글꼴 열거'
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- typography [WPF], enumerating system fonts
- fonts [WPF], enumerating
- system fonts [WPF], enumerating
- enumerating [WPF], system fonts
ms.assetid: 36e37791-55b9-4f01-a496-5cc10335e6a6
ms.openlocfilehash: 7fc996a2d3ba7042fce70afc20be5d64042c2b63
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
ms.locfileid: "33543757"
---
# <a name="how-to-enumerate-system-fonts"></a>방법: 시스템 글꼴 열거
## <a name="example"></a>예제  
 다음 예제에서는 시스템 글꼴 컬렉션에서 글꼴을 열거 하는 방법을 보여 줍니다. 각각의 글꼴 패밀리 이름을 <xref:System.Windows.Media.FontFamily> 내 <xref:System.Windows.Media.Fonts.SystemFontFamilies%2A> 콤보 상자에 항목으로 추가 됩니다.  
  
 [!code-csharp[TextOverview#100](../../../../samples/snippets/csharp/VS_Snippets_Wpf/TextOverview/CSharp/Window1.xaml.cs#100)]
 [!code-vb[TextOverview#100](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/TextOverview/visualbasic/window1.xaml.vb#100)]  
  
 같은 디렉터리에 있는 여러 버전의 동일한 글꼴 패밀리는 [!INCLUDE[TLA#tla_winclient](../../../../includes/tlasharptla-winclient-md.md)] 글꼴 열거형 글꼴의 가장 최신 버전을 반환 합니다. 버전 정보 확인을 제공 하지 않는 경우 최신 타임 스탬프가 있는 글꼴 반환 됩니다. 타임 스탬프 정보를 해당 하는 경우에 알파벳 순서로 첫 번째 글꼴 파일이 반환 됩니다.
