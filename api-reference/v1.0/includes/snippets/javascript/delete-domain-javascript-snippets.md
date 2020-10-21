---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e0c692776d86b734b2d8b93083f083d22dfd047f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com')
    .delete();

```