---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 26dd39e2a3b998f6a4133a9d7a395d9c3f8ac65f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const insightsSettings = {
  isEnabledInOrganization: true,
  disabledForGroup: 'edbfe4fb-ec70-4300-928f-dbb2ae86c981'
};

await client.api('/organization/{organizationId}/settings/peopleInsights')
    .version('beta')
    .update(insightsSettings);

```