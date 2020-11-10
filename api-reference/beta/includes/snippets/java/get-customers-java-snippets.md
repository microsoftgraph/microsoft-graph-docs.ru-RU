---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 43f78a43b4be3db290369259f1d0b917cee54c1b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960816"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IBookingCustomerCollectionPage customers = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers()
    .buildRequest()
    .get();

```