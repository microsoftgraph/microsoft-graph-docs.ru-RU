---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1b1e2d4aa138ffc0cece092808ee757e88c75819
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits/{id}')
    .version('beta')
    .delete();

```