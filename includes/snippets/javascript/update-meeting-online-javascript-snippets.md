---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ddf58074cdcad8b25d9b7197bf685cc9df4ece52
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39637030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  isOnlineMeeting: true,
  onlineMeetingProvider: "teamsForBusiness"
};

let res = await client.api('/me/events/AAMkADAGu0AABIGYDaAAA=')
    .version('beta')
    .update(event);

```