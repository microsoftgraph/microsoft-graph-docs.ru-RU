---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3296600f1274adb0b6b0443625c4a36d717b0f81f2e3dadbca2058c8682e60d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050579"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onlineMeetings = await client.api('/communications/onlineMeetings/')
    .version('beta')
    .filter('VideoTeleconferenceId eq \'123456789\'')
    .get();

```