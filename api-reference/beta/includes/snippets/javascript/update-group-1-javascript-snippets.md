---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f3133ba36d9d3b17733597107950f02ec1609155
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53444315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
   description: 'Contoso Life v2.0',
   displayName: 'Contoso Life Renewed'
};

await client.api('/groups/{id}')
    .version('beta')
    .update(group);

```