---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5bbe23e38b5839687c536344b7f38ce0f47df6957f6dfd20e21829d175911d31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57250700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let site = await client.api('/sites/{site-id}')
    .get();

```