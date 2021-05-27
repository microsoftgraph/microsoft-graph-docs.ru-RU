---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae6107c2be8700365e8d00ef22d4bf8e509fa9e7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taughtClasses = await client.api('/education/classes/{educationClassId}/members/{educationUserId}/taughtClasses')
    .get();

```