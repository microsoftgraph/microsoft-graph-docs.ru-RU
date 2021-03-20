---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ccf0f4af9569c4362810a7814742893aeb08cb5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/groups/{group-id}/planner/plans')
    .get();

```