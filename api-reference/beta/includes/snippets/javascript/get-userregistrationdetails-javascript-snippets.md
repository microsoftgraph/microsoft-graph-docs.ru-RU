---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8e3db8db7c27d78bb9305d1aadfbc48d542979f0
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userRegistrationDetails = await client.api('/reports/authenticationMethods/userRegistrationDetails/{userRegistrationDetailsId}')
    .version('beta')
    .get();

```