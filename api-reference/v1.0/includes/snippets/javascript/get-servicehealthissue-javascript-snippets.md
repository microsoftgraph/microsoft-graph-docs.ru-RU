---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0789d77e3fd0bfed16a1581f23730ca6a4368ba6
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceHealthIssue = await client.api('/admin/serviceAnnouncement/issues/MO226784')
    .get();

```