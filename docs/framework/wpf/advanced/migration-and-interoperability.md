---
title: "마이그레이션 및 상호 운용성 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-wpf"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "AutoGeneratedOrientationPage"
helpviewer_keywords: 
  - "컨트롤[WPF 상호 운용성]"
  - "상호 운용성[WPF]"
  - "마이그레이션[WPF]"
  - "Windows Forms 컨트롤[WPF 상호 운용성]"
  - "Windows Presentation Foundation, 상호 운용성"
  - "Windows Presentation Foundation, 마이그레이션"
  - "WPF, 상호 운용성"
  - "WPF, 마이그레이션"
ms.assetid: d655de05-bf63-4814-bc64-6b3be01c70a2
caps.latest.revision: 41
author: "dotnet-bot"
ms.author: "dotnetcontent"
manager: "wpickett"
caps.handback.revision: 41
---
# 마이그레이션 및 상호 운용성
이 페이지에는 [!INCLUDE[TLA#tla_winclient](../../../../includes/tlasharptla-winclient-md.md)] 응용 프로그램 및 다른 [!INCLUDE[TLA#tla_win](../../../../includes/tlasharptla-win-md.md)] 응용 프로그램 형식 간 상호 운용을 구현하는 방법을 설명하는 문서에 대한 링크가 포함되어 있습니다.  
  
## 단원 내용  
 [WPF 및 Windows Forms 상호 운용성](../../../../docs/framework/wpf/advanced/wpf-and-windows-forms-interoperation.md)  
 [WPF 및 Win32 상호 운용성](../../../../docs/framework/wpf/advanced/wpf-and-win32-interoperation.md)  
 [WPF 및 Direct3D9 상호 운용성](../../../../docs/framework/wpf/advanced/wpf-and-direct3d9-interoperation.md)  
  
## 참조  
  
|용어|정의|  
|--------|--------|  
|<xref:System.Windows.Forms.Integration.WindowsFormsHost>|[!INCLUDE[TLA#tla_winforms](../../../../includes/tlasharptla-winforms-md.md)] 컨트롤을 [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 페이지의 요소로 호스팅하는 데 사용할 수 있는 요소입니다.|  
|<xref:System.Windows.Forms.Integration.ElementHost>|[!INCLUDE[TLA#tla_winclient](../../../../includes/tlasharptla-winclient-md.md)] 컨트롤을 호스팅하는 데 사용할 수 있는 [!INCLUDE[TLA#tla_winforms](../../../../includes/tlasharptla-winforms-md.md)] 컨트롤입니다.|  
|<xref:System.Windows.Interop.HwndSource>|[!INCLUDE[TLA2#tla_win32](../../../../includes/tla2sharptla-win32-md.md)] 응용 프로그램 내에서 [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 영역을 호스팅합니다.|  
|<xref:System.Windows.Interop.HwndHost>|<xref:System.Windows.Forms.Integration.WindowsFormsHost>의 기본 클래스로, [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 응용 프로그램에 의해 호스팅될 때 모든 HWND 기반 기술에서 사용하는 몇 가지 기본 기능을 정의합니다.  [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 응용 프로그램 내에서 [!INCLUDE[TLA2#tla_win32](../../../../includes/tla2sharptla-win32-md.md)] 창을 호스팅하기 위해 이 클래스의 서브클래스를 생성합니다.|  
|<xref:System.Windows.Interop.BrowserInteropHelper>|브라우저에 의해 호스팅되는 [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 응용 프로그램의 브라우저 환경의 상태를 보고하는 도우미 클래스입니다.|  
  
## 관련 단원