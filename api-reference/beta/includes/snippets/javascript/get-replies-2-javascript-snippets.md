---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d29a140b2929605497fc2d6c68c4a7ee9615aecf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let replies = await client.api('/drive/items/{id}/workbook/comments/{id}/replies')
    .version('beta')
    .get();

```