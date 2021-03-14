---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 56836f44ab291e56af1824d062783b23ed7d8ca2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookCommentReply = await client.api('/drive/items/{id}/workbook/comments/{id}/replies/{id}')
    .get();

```