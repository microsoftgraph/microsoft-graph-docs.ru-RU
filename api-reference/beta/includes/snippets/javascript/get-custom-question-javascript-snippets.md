---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4f05c22b2f0366f122dc83939805c141bd959955
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let meetingRegistrationQuestion = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions/MSMxY2E2ZmE3OS1hOTY3LTQ4ZX3lvdV94MDAyMF9hX3gwMDIwX2RldmU=')
    .version('beta')
    .get();

```