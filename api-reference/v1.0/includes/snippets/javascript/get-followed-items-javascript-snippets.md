---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c1ca75f72b5302a9964a1f7d0a318609eaed5dfa67e900e15f7befdce4b78d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let following = await client.api('/me/drive/following')
    .get();

```