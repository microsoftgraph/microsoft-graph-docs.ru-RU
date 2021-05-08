---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cd66e1680196cb26017651e871964472c79807ef
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviewPolicy = await client.api('/identityGovernance/accessReviews/policy')
    .version('beta')
    .get();

```