---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fe61add9bae0487004a02207b994f4b45e9f5bbb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantsOperation = {
  participants: [
    ''
  ],
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/{id}/participants/muteAll')
    .version('beta')
    .post(muteParticipantsOperation);

```