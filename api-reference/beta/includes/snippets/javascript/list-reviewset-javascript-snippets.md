---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 391e9801994cea23b3414fc5a68f4319b6cf5e20161e28b837e29025c8cc4ded
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57249658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let reviewSets = await client.api('/compliance/ediscovery/cases/{caseId}/reviewSets')
    .version('beta')
    .get();

```