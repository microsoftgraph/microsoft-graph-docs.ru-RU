---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2213847f2c2ec2de2a70d80baa97af67bd8729ec
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let catalogs = await client.api('/identityGovernance/entitlementManagement/catalogs')
    .get();

```