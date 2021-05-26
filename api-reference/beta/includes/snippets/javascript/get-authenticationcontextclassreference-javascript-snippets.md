---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d274b4aaee83f749622c5e02d518f9f94402bc9
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationContextClassReferences = await client.api('/identity/conditionalAccess/authenticationContextClassReferences')
    .version('beta')
    .get();

```