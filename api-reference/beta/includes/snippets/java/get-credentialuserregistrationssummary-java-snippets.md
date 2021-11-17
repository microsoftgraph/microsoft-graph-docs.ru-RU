---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 879e4c36429107d4882136e07bbf73b6d1d9d2a35750738596a3b969361522b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57262622"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CredentialUserRegistrationsSummary credentialUserRegistrationsSummary = graphClient.tenantRelationships().managedTenants().credentialUserRegistrationsSummaries("{credentialUserRegistrationsSummaryId}")
    .buildRequest()
    .get();

```