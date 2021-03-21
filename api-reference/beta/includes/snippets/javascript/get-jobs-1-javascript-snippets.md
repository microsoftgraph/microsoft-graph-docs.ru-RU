---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f0fd0dbf2e5575a4563877f092fca97888303512
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let jobs = await client.api('/print/printers/{id}/jobs')
    .version('beta')
    .get();

```