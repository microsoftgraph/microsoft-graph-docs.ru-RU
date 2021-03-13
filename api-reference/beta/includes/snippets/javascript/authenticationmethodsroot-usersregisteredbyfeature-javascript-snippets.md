---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ddd8890496eb3c26727237c3082bcf00d3da6782
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userRegistrationFeatureSummary = await client.api('/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')')
    .version('beta')
    .get();

```