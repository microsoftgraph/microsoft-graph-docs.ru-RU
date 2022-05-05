---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07c9933860d65f85351b3d648ead3fd49cf99978
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/bundles/{bundle-id}/children/{item-id}')
    .delete();

```