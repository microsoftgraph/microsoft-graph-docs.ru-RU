---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0dc066093714f24554f455f55981efab07a91f3b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let fido2AuthenticationMethod = await client.api('/me/authentication/fido2Methods/-2_GRUg2-HYz6_1YG4YRAQ2')
    .version('beta')
    .get();

```