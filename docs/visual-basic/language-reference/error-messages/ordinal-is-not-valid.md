---
title: 서수가 잘못되었습니다.
ms.date: 07/20/2015
f1_keywords:
- vbrID452
ms.assetid: 7459562b-cd4f-4590-95e0-6126ae3589a5
ms.openlocfilehash: 12d73b33e3c025b40c98d84e3507af7be1e1e91a
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/04/2018
ms.locfileid: "33593605"
---
# <a name="ordinal-is-not-valid"></a>서수가 잘못되었습니다.
프로시저 이름 대신 숫자를 사용 하는 동적 연결 라이브러리 (DLL)를 호출 하 여 표시를 사용 하는 `#num` 구문입니다. 이 오류는 다음과 같은 가능한 원인을 있습니다.  
  
-   변환할 수는 `#num` 식 실패 하는 서 수입니다.  
  
-   `#num` 지정 된 DLL의 함수를 지정 하지 않습니다.  
  
-   형식 라이브러리에 잘못 된 서 수의 내부 사용에 잘못 된 선언이 있습니다.  
  
## <a name="to-correct-this-error"></a>이 오류를 해결하려면  
  
1.  식이 올바른 숫자를 나타내는 있는지 확인 하거나 이름별으로 프로시저를 호출 합니다.  
  
2.  확인 `#num` DLL의 올바른 함수를 식별 합니다.  
  
3.  코드를 주석 처리 문제를 발생 시키는 프로시저 호출을 격리 합니다. 작성 한 `Declare` 프로시저와 보고서 문제를 형식 라이브러리 공급 업체에 문의 합니다.  
  
## <a name="see-also"></a>참고 항목  
 [Declare 문](../../../visual-basic/language-reference/statements/declare-statement.md)
