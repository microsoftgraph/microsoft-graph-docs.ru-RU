---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c21e7013412bf18231b29e1a803a4e0a4419d404986493d56636a0b2c0503013
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57198929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/users/13019')
    .version('beta')
    .delete();

```