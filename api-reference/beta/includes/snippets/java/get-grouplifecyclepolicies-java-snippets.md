---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee2bda31f57dd6425843d1cc216bfa7f8300e7dd2e19e24e19be32bc3a9a661d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57247656"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicyCollectionPage groupLifecyclePolicies = graphClient.groups("{id}").groupLifecyclePolicies()
    .buildRequest()
    .get();

```