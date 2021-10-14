---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d268e7d1fa37ecaf4e90810cf2f4590f0a01db97ea71f3e6899a337d4e3ea6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let usageRights = await client.api('/devices/{objectId}/usageRights')
    .version('beta')
    .filter('state in (\'active\', \'suspended\') and serviceIdentifier in (\'ABCD\')')
    .get();

```