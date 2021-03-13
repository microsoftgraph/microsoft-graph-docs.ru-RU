---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c590a867288f19dab4f7a08a6de4ce9f69b8b083
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequests = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .get();

```