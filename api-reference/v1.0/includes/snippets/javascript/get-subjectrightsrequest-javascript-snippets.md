---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 86c42df2d80b30407d4086fe8377f31385d188b6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subjectRightsRequest = await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}')
    .get();

```