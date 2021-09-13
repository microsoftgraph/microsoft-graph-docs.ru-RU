---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ade1d33f579dd0f6548f574b12a50396f53cdc19fc7d7d7b4798a00f1769bae3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/me/drive')
    .get();

```