---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff5f35006a6860f6ec9c0dcb45d069a59650a7e8952eb06b7e199b812d864f96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051910"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const confirmCompromised = {
  userIds: [
    '29f270bb-4d23-4f68-8a57-dc73dc0d4caf',
    '20f91ec9-d140-4d90-9cd9-f618587a1471'
  ]
};

await client.api('/riskyUsers/confirmCompromised')
    .version('beta')
    .post(confirmCompromised);

```