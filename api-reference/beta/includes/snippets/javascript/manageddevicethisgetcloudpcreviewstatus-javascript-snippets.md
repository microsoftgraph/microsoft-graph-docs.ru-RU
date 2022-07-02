---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 978f76cb952667c6f0aebd1c9dc0f005f918f7cd
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcReviewStatus = await client.api('/deviceManagement/managedDevices/185f01c2de954929afb129392e5d9f47/getCloudPcReviewStatus')
    .version('beta')
    .get();

```