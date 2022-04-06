---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 41554d5f9f053efbd15328cb50a980382e3e8bdb
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bundles = await client.api('/drive/bundles?filter=bundle/album%20ne%20null')
    .version('beta')
    .filter('bundle/album ne null')
    .get();

```