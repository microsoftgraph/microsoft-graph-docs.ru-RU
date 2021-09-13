---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c466e13502d0979699dd6ddb773bdafa2a9a5abe3c710b675820a0dc0de5f29b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57153030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/domains/{domain-name}/verify')
    .post();

```