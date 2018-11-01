---
title: 오픈 소스 라이브러리 지침
description: 고품질 .NET 라이브러리를 만드는 개발자를 위한 모범 사례 권장 사항입니다.
author: jamesnk
ms.author: mairaw
ms.date: 10/17/2018
ms.openlocfilehash: ca95cb5ba1ebf27464397b7850ac02aabded1a5b
ms.sourcegitcommit: c93fd5139f9efcf6db514e3474301738a6d1d649
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/27/2018
ms.locfileid: "50188627"
---
# <a name="open-source-library-guidance"></a>오픈 소스 라이브러리 지침

이 지침에서는 고품질 .NET 라이브러리를 만드는 개발자를 위한 권장 사항을 제공합니다. 이 설명서는 .NET 라이브러리를 빌드하는 경우 *방법*이 아닌 *내용* 및 *이유*에 중점을 둡니다.

고품질 오픈 소스 .NET 라이브러리의 측면:

> [!div class="checklist"]
> * **포괄적** - 우수한 .NET 라이브러리는 여러 플랫폼, 프로그래밍 언어 및 응용 프로그램을 지원하기 위해 노력합니다.
> * **안정적** - 우수한 .NET 라이브러리는 에코시스템에서 공존하며 다양한 라이브러리를 사용하여 빌드된 응용 프로그램에서 실행됩니다.
> * **진화하도록 설계** - .NET 라이브러리는 시간이 지남에 따라 개선되고 진화하는 동시에 기존 사용자를 지원해야 합니다.
> * **디버깅 가능** - .NET 라이브러리는 사용자에 대해 뛰어난 디버깅 환경을 만드는 최신 도구를 사용해야 합니다.
> * **신뢰할 수 있음** - .NET 라이브러리는 보안 모범 사례를 사용하는 NuGet에 게시하여 개발자의 신뢰를 얻고 있습니다.

> [!div class="nextstepaction"]
> [시작](./get-started.md)

## <a name="types-of-recommendations"></a>권장 사항 유형

각 문서에서는 **수행**, **고려**, **회피** 및 **금지**의 네 가지 권장 사항 유형을 제공합니다. 각 권장 사항 유형은 수행해야 하는 필요성의 정도를 나타냅니다.

**수행** 권장 사항은 거의 항상 따라야 합니다. 예:

**✔️ 수행** NuGet 패키지를 사용하여 라이브러리를 배포합니다.

한편으로 **고려** 권장 사항은 일반적으로 따라야 하지만 규칙에 대한 정당한 예외가 있거나 지침을 따르지 않아도 됩니다.

**✔️ 고려** [SemVer 2.0.0](https://semver.org/)을 사용하여 NuGet 패키지 버전을 관리합니다.

**회피** 권장 사항은 일반적으로 좋지는 않지만 규칙을 깨는 것이 적합한 경우를 언급합니다.

**❌ 회피** 정확한 버전을 요구하는 NuGet 패키지 참조입니다.

마지막으로, **금지**는 수행하지 않아야 하는 항목을 나타냅니다.

**❌ 금지** 강력한 이름이 지정되고 강력하지 않은 이름이 지정된 버전의 라이브러리를 게시합니다. 예를 들어 `Contoso.Api` 및 `Contoso.Api.StrongNamed`를 지정합니다.

>[!div class="step-by-step"]
[다음](./get-started.md)