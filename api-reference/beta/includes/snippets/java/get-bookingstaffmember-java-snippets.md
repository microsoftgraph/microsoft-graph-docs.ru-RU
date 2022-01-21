---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e1774271e9142dcfa71380448049c931aaaf5ac3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116396"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingStaffMember bookingStaffMember = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").staffMembers("71d64d0e-7225-49b6-b0b1-070d476cda51")
    .buildRequest()
    .get();

```