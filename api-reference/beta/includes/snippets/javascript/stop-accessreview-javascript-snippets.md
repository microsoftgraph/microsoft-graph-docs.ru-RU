---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 20fc632e0298b0590a00b2f3ae78905310abfadba0411ef6eae3867797ff3a6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop')
    .version('beta')
    .post();

```