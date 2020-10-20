---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2021a16a44ef2a75abf1f5349351d056ab91589e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls')
    .version('beta')
    .get();

```