---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d2ec7552d95bf1968374737f2bee4b4ae94dc760110ce98247bc873832c97776
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/decisions/filterByCurrentUser(on='reviewer')')
    .version('beta')
    .get();

```