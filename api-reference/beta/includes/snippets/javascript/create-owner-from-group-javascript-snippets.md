---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c360b58bdc93b9424e7c6bc4c1ef020cf8568b13df8e32a14ce4466644f2a24d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57142054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/users/{id}'
};

await client.api('/groups/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```