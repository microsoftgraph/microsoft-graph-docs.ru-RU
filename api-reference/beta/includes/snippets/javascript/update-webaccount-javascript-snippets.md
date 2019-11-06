---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 691936c9d44c7ecb0c8181e64a11ea78538d7e0e
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const webAccount = {
  description: "description-value",
  userId: "userId-value",
  service: {
    name: "name-value",
    webUrl: "webUrl-value"
  },
  statusMessage: "statusMessage-value",
  webUrl: "webUrl-value"
};

let res = await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .update(webAccount);

```