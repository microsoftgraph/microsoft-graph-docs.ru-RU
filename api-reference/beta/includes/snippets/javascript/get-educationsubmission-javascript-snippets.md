---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03bbbfc066a1ea1bfec8c66eb5e4abeb55096f8f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSubmission = await client.api('/education/classes/59069eb2-2a09-4d90-bb19-2089cc69d613/assignments/80da1069-a635-4913-813f-d775a5470a8f/submissions/869369de-3e5a-89eb-6f2d-83cd88f860b5')
    .version('beta')
    .get();

```