---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8069e6ce7e2c35067c9f13b8439ec6e62cf6f06b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/incomingChannels/19:56eb04e133944cf69e603c5dac2d292e@thread.skype/$ref')
    .version('beta')
    .delete();

```