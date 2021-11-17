---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e77b9c95a19c58dfc3307fd3710c2d1a20711686158efccaba2d1d7027973d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57314640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let homeRealmDiscoveryPolicies = await client.api('/policies/homeRealmDiscoveryPolicies')
    .version('beta')
    .get();

```