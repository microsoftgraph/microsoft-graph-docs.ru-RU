---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 58c6087e29e975918b39ab89fcc3f96ca91de69ef13213bdfb405ee46d8e2397
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57251679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: 'Volunteer'
};

await client.api('/me/calendars')
    .version('beta')
    .post(calendar);

```