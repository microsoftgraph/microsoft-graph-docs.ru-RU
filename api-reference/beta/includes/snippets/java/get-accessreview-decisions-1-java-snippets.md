---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ceff0207b43e3b29e7f07188abeaef5639a63a33cede2f50143fe9127172782a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051207"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewDecisionCollectionPage decisions = graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").decisions()
    .buildRequest()
    .get();

```