---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 658bc7c74eff691e4293857c0bcae0b3db97aab3d58cdfe90e960a173e2974a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57202124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printer = await client.api('/print/printers/{id}')
    .version('beta')
    .get();

```