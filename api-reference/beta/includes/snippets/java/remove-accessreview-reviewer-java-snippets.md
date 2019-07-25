---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fadd62df886c34965d6802323e9aed5c6b888aec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856030"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").reviewers("006111db-0810-4494-a6df-904d368bd81b")
    .buildRequest()
    .delete();

```