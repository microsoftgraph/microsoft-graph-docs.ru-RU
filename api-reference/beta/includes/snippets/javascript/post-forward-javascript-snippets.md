---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b409edb4a89fe0aa656d34f5100e1b5f3ed2f874383aee08bc7379b4d20bd29d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57209903"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  comment: 'comment-value',
  toRecipients: [
    {
      emailAddress: {
        name: 'name-value',
        address: 'address-value'
      }
    }
  ]
};

await client.api('/groups/{id}/threads/{id}/posts/{id}/forward')
    .version('beta')
    .post(forward);

```