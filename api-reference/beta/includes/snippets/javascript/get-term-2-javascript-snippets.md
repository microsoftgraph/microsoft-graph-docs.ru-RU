---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0eeb94b3cbd1118359a6acf46d579c43c3c38a2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/termStore/sets/{setId}/children')
    .version('beta')
    .get();

```