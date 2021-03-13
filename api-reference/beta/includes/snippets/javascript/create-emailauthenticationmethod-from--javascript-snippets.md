---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9c7022ff6fb52b31be79192dda9da3a5e3cb084b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const emailAuthenticationMethod = {
  emailAddress: 'kim@contoso.com'
};

await client.api('/users/kim@contoso.com/authentication/emailMethods')
    .version('beta')
    .post(emailAuthenticationMethod);

```