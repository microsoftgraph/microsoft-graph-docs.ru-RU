---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 88fac22c23af8d5d6289696466f8364a041a2622
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  parentFolderId: "parentFolderId-value",
  birthday: "datetime-value",
  fileAs: "fileAs-value",
  displayName: "displayName-value",
  givenName: "givenName-value",
  initials: "initials-value"
};

let res = await client.api('/me/contactFolders/{id}/contacts')
    .post(contact);

```