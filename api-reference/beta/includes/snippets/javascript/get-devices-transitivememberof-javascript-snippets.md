---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 40c2801721fe7dd400442f7bbd7ed9fbf83f1895e553cb8558e0b90b2fe0f554
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57259025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/devices/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```