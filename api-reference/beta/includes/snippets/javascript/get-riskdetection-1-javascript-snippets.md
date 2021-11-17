---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14a822c9073117e8612ba7824f7e8cb9527011254daf9cab1872ddbf371d83e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57203972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetections = await client.api('/riskDetections')
    .version('beta')
    .get();

```