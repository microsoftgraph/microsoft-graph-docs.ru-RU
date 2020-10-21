---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5be5741b63ac25fcd298bfc1cd9613147a75b842
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610099"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryObjects/{id}')
    .delete();

```