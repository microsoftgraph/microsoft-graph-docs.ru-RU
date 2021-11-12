---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 59179c4702550f56e91fc4a476fedc2453a01d946f135eac96db88342284dfe4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: 'destinationId-value'
};

await client.api('/me/mailFolders/{id}/move')
    .version('beta')
    .post(mailFolder);

```