---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eb973f8660cbbfafa582e1aa987082d82a7809342b9398f7066dfa534d154cf5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const listItem = {
  fields: {
    Title: 'Widget',
    Color: 'Purple',
    Weight: 32
  }
};

await client.api('/sites/{site-id}/lists/{list-id}/items')
    .version('beta')
    .post(listItem);

```