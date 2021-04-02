---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 01a7f14a81e93afbde0e4b5c40f8102d59d087f9
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507271"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  displayName: 'Family'
};

await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .post(contactFolder);

```