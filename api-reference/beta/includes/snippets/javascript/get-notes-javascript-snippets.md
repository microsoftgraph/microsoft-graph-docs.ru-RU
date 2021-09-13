---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d527cfc5b0c9b33f7ec579687270c7a52f545a1fdd74ac81de32a3ea40840aa7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57204112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notes = await client.api('/me/profile/notes')
    .version('beta')
    .get();

```