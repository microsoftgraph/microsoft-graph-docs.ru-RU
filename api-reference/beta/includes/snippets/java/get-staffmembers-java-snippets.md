---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 673b2066a879fa369eee7979f0e35fea0aac40a3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106949"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingStaffMemberCollectionPage staffMembers = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").staffMembers()
    .buildRequest()
    .get();

```