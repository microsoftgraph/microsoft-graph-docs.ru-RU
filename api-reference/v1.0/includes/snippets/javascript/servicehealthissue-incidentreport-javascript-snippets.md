---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 54a29045f2e691e279864eb5e5adfd1de3b1bd55
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/admin/serviceAnnouncement/issues/MO248163/incidentReport')
    .get();

```