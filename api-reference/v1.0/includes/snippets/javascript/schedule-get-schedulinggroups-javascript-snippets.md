---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 16b67f1521a10aa83a921a1c72cd40bde463a818b545a86ba96465ee703734a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57432235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schedulingGroup = await client.api('/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}')
    .get();

```