---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 23f923f0b0fc231c58c8f63bd6b861f5f8acbd24
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attributeSet = {
    id: 'Engineering',
    description: 'Attributes for engineering team',
    maxAttributesPerSet: 25
};

await client.api('/directory/attributeSets')
    .version('beta')
    .post(attributeSet);

```