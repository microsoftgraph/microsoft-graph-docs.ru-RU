---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0955d2d78845b3692895d128453a8d9cce216b10f32aeae436b6027ce2ca116e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57311799"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedulingGroups = await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .get();

```