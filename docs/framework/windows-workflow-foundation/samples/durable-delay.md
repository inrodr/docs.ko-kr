---
title: "Durable Delay | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 220ec240-b958-430c-81ff-b734a6aa97ae
caps.latest.revision: 11
author: "Erikre"
ms.author: "erikre"
manager: "erikre"
caps.handback.revision: 11
---
# Durable Delay
이 샘플에서는 지속적 지연을 사용하는 방법을 보여 줍니다. 지속적 지연은 지연 중 워크플로를 영구적인 장치에 저장하는 지연입니다.샘플 워크플로에는 지연으로 구분되는 콘솔 대상의 두 메시지가 포함되어 있습니다.지연이 트리거되면 워크플로가 언로드된 다음 워크플로 인스턴스 저장소에서 5초 동안 기다렸다가 메모리에 다시 로드됩니다.  
  
## 워크플로 세부 정보  
 워크플로 서비스 호스트에서는 워크플로를 호스팅할 뿐 아니라 워크플로 인스턴스를 로드하거나 언로드하여 워크플로 인스턴스를 관리합니다.워크플로 정의의 인스턴스를 시작하기 위해 이 샘플에서는 워크플로의 <xref:System.ServiceModel.Activities.Receive> 활동에 메시지를 보내는 프록시를 설정합니다.<xref:System.ServiceModel.Activities.Receive.CanCreateInstance%2A> 속성이 `true`로 설정되어 있으므로 이 활동에서는 메시지를 받으면 워크플로의 새 인스턴스를 만들 수 있습니다.  
  
 다음 목록에서는 초기화 중 워크플로 서비스에 의한 설정 과정을 자세히 설명합니다.  
  
1.  주소가 http:\/\/localhost:8080\/Client인 서비스 호스트를 만듭니다.  
  
2.  워크플로 내의 <xref:System.ServiceModel.Activities.Receive> 활동과 통신할 수 있도록 서비스 호스트에 끝점을 만듭니다.  
  
3.  SQL 인스턴스 저장소를 설정합니다.  
  
4.  워크플로 서비스 호스트에서 워크플로 인스턴스를 SQL 지속성 저장소로 언로드할 조건을 지정하는 언로드 인스턴스 동작을 추가합니다.이 샘플의 경우에는 지연이 트리거되어 워크플로가 유휴 상태가 된 직후에 인스턴스를 언로드합니다.  
  
5.  워크플로의 <xref:System.ServiceModel.Activities.Receive> 활동에 메시지를 보내는 프록시를 만듭니다.  
  
#### 이 샘플을 사용하려면  
  
1.  지속성 데이터베이스를 설치합니다.  
  
    1.  [!INCLUDE[vs2010](../../../../includes/vs2010-md.md)] 명령 프롬프트를 엽니다.  
  
    2.  [!INCLUDE[dnprdnshort](../../../../includes/dnprdnshort-md.md)] 디렉터리\(C:\\Windows\\Microsoft.NET\\Framework\\v4.X\\\)로 이동합니다.  
  
    3.  WorkflowManagementService.exe.config 파일을 편집하고 다음 연결 문자열을 \<`database`\> 요소 내에 추가합니다.  
  
        ```  
        <database connectionString="Data Source=localhost\SQLEXPRESS;Initial Catalog=DefaultSampleStore;Integrated Security=True;Asynchronous Processing=True" />  
  
        ```  
  
    4.  DurableDelay\\CS 디렉터리로 이동합니다.  
  
    5.  Setup.cmd를 실행합니다.  
  
2.  [!INCLUDE[vs2010](../../../../includes/vs2010-md.md)] 아이콘을 마우스 오른쪽 단추로 클릭하고 **관리자 권한으로 실행**을 선택하여 높은 권한으로 [!INCLUDE[vs2010](../../../../includes/vs2010-md.md)]을 실행합니다.  
  
3.  Delay.sln 솔루션 파일을 엽니다.  
  
4.  Ctrl\+Shift\+B를 눌러 솔루션을 빌드합니다.  
  
5.  Ctrl\+F5를 눌러 솔루션을 실행합니다.  
  
#### 이 샘플을 제거하려면  
  
1.  [!INCLUDE[vs2010](../../../../includes/vs2010-md.md)] 명령 프롬프트를 엽니다.  
  
2.  DurableDelay\\CS 디렉터리로 이동합니다.  
  
3.  Cleanup.cmd를 실행합니다.  
  
> [!IMPORTANT]
>  컴퓨터에 이 샘플이 이미 설치되어 있을 수도 있습니다.계속하기 전에 다음\(기본\) 디렉터리를 확인하십시오.  
>   
>  `<InstallDrive>:\WF_WCF_Samples`  
>   
>  이 디렉터리가 없으면 [Windows Communication Foundation \(WCF\) and Windows Workflow Foundation \(WF\) Samples for .NET Framework 4](http://go.microsoft.com/fwlink/?LinkId=150780)로 이동하여 [!INCLUDE[indigo1](../../../../includes/indigo1-md.md)] 및 [!INCLUDE[wf1](../../../../includes/wf1-md.md)] 샘플을 모두 다운로드하십시오.이 샘플은 다음 디렉터리에 있습니다.  
>   
>  `<InstallDrive>:\WF_WCF_Samples\WF\Basic\Services\DurableDelay`  
  
## 참고 항목