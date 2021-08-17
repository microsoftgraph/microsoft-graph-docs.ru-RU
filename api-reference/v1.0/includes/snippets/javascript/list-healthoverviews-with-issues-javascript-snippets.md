---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0be88400542381ed2eaf38ea1d051c653fafe203
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259147"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let healthOverviews = await client.api('/admin/serviceAnnouncement/healthOverviews')
    .expand('issues')
    .get();

```