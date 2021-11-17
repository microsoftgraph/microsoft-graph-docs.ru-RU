---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1b913a7954563c7e3a68050eb5f0e8c2634fbf355b864cad09fc3e04be6160c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57318920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let phones = await client.api('/me/profile/phones')
    .version('beta')
    .get();

```