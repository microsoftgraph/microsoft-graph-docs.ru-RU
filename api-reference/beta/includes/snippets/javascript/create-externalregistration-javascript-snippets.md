---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0d3de55b3c98b2fbf345eb71a9f01cbb30e87295
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistration = {
  '@odata.type': '#microsoft.graph.externalMeetingRegistration',
  allowedRegistrant: 'everyone'
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration')
    .version('beta')
    .post(meetingRegistration);

```