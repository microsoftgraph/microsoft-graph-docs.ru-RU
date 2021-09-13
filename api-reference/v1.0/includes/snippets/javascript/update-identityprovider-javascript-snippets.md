---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c61bd6d8fbb80cb4ee0344bbee998b0d39b8866e358b9fe7cfd6dcbd15f655a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57259256"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
    clientSecret: '1111111111111'
};

await client.api('/identityProviders/Amazon-OAuth')
    .update(identityProvider);

```