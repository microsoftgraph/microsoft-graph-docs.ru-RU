---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6f70ff757e7f0d3d29d4b370445f29ba4102a4ca4cb4a8c0494f33572220334f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394205"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let swapShiftsChangeRequests = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests')
    .get();

```