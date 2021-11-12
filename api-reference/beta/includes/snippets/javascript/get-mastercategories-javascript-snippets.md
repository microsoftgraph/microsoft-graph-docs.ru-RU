---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d16fef3ccfcd733a4fb92088a51aa25df408f0dbedeea81b0ad5c16a06357a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57309494"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let masterCategories = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .get();

```