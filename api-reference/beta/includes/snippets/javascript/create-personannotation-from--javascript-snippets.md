---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b99ac8431db2e3e3cda567577a7997b416bcaa13
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnotation = {
  detail: {
    contentType: 'text',
    content: 'I am originally from Australia, but grew up in Moscow, Russia.'
  },
  displayName: 'About Me'
};

await client.api('/me/profile/notes')
    .version('beta')
    .post(personAnnotation);

```