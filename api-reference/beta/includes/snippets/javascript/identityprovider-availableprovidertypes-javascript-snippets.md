---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c9fe08affd9b65ce65f27d19cab3aec1b0c866c0
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52684229"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let availableProviderTypes = await client.api('/identity/identityProviders/availableProviderTypes')
    .version('beta')
    .get();

```