---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 92e1f0aff39ad35b08b266b4475a84e770e5012d
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853318"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceDecisionItem accessReviewInstanceDecisionItem = graphClient.identityGovernance().accessReviews().definitions("5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0").instances("6444d4fd-ab55-4608-8cf9-c6702d172bcc").stages("9458f255-dff2-4d86-9a05-69438f49d7f8").decisions("e6cafba0-cbf0-4748-8868-0810c7f4cc06")
    .buildRequest()
    .get();

```