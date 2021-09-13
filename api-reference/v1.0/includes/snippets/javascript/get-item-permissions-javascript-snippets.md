---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3c57ff294ce39ebe6a1755b4a036dbd08a06263c0182077ed5f79c6a95407f02
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57429352"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissions = await client.api('/me/drive/items/{item-id}/permissions')
    .get();

```