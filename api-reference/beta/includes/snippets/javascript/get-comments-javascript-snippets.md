---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a2c75bf14c3efe32d64584b3f85f38cc6c30509065474e5075148602f371afe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57212475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let comments = await client.api('/drive/items/{id}/workbook/comments')
    .version('beta')
    .get();

```