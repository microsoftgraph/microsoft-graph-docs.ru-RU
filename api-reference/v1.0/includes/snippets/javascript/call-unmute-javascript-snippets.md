---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8a0bafa40cd26048047053ba4e56c4a801b65de590d2d31f69f352c8486b200f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57433054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unmuteParticipantOperation = {
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute')
    .post(unmuteParticipantOperation);

```