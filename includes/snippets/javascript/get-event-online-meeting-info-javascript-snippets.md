---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e8fbd637caa539026ec19e47d4915639b5f7516
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39637024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkADAGu0AABIGYDZAAA=')
    .version('beta')
    .select('isOnlineMeeting,onlineMeetingProvider,onlineMeeting')
    .get();

```