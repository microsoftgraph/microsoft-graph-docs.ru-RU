---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b389c27441502a3377ff5d26d343f39b0e49d838
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettings')
    .get();

```