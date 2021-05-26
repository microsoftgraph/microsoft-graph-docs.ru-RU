---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: da42bad6116650caa5a5873c02b37b40aa2bb7f8
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationContextClassReference = {
    id: 'c1',
    displayName: 'Contoso medium',
    description: 'Medium protection level defined for Contoso policy',
    isAvailable: true
};

await client.api('/identity/conditionalAccess/authenticationContextClassReferences')
    .version('beta')
    .post(authenticationContextClassReference);

```