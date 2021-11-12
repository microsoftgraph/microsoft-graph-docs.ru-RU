---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 05b177047c4813fa077862450e27d7c963e552bb13199b2cb2c9f36c375522c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57254836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printSettings = await client.api('/print/settings')
    .get();

```