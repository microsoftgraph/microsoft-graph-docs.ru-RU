---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e568250a2e310cb0261be2269e338135c3a686c57a5040d8315f03cb1d515fd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141303"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-id}')
    .get();

```