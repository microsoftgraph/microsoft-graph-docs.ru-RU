---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1933b9ab220f2830d76ecc4cdce3a1f6d99f16f857861f1d64a36801db0a830
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookTaskGroup = await client.api('/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .get();

```