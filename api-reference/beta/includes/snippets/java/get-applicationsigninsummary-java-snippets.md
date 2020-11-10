---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7632eb33a3c6aab7fefb9f9c4c9a16cd9c3d572d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961806"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IReportRootGetAzureADApplicationSignInSummaryCollectionPage getAzureADApplicationSignInSummary = graphClient.reports()
    .getAzureADApplicationSignInSummary("D7")
    .buildRequest()
    .get();

```