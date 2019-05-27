---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 35b88d21c7f7f6fc59e72e629de0c670ab46c130
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475628"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  @odata.type:"#Microsoft.OutlookServices.ConversationThread",
  isLocked: true
};

let res = await client.api('/groups/{id}/threads/{id}')
    .update({conversationThread : conversationThread});

```