---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f20c0a530c496759f97a40f4fed30fe4b9cc336b40aff2e6a12c94cd56ead9b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printJob = await client.api('/print/printers/c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb/jobs/5182')
    .version('beta')
    .get();

```