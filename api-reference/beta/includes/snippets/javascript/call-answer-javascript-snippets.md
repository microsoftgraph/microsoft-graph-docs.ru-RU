---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03ae202e65c8160586ddb0843e3b8c60d583aa58
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220697"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: 'callbackUri-value',
  mediaConfig: {
    '@odata.type': '#microsoft.graph.appHostedMediaConfig',
    blob: '<Media Session Configuration Blob>'
  },
  acceptedModalities: [
    'audio'
  ],
  callOptions: {
    '@odata.type': '#microsoft.graph.incomingCallOptions',
    isContentSharingNotificationEnabled: true
  },
  participantCapacity: 200
};

await client.api('/communications/calls/{id}/answer')
    .version('beta')
    .post(answer);

```