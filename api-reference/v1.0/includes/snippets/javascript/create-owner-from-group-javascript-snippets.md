---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d5de356a39481e78d4cb6f187b522300f0b07afa20a7141e22e42cfbcc368dbf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57372338"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/users/{id}'
};

await client.api('/groups/{id}/owners/$ref')
    .post(directoryObject);

```