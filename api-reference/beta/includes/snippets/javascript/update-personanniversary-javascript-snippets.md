---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8567c0b1b1e04f565367a2d30db5d2831adb705b733b411aa15d95438a8f69f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnualEvent = {
  allowedAudiences: 'contacts'
};

await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .update(personAnnualEvent);

```