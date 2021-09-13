---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 527e753870ffdcfba79556c1765cb77adeef39838a0ed8965f1b670a54e8abfa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57318080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')')
    .filter('userConsentRequests/any(u:u/status eq \'InProgress\')')
    .get();

```