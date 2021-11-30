---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9fba762a3cc5de31b4abf42660db0cfaca62c315
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226816"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const customSecurityAttributeDefinition = {
    attributeSet: 'Engineering',
    description: 'Target completion date',
    isCollection: false,
    isSearchable: true,
    name: 'ProjectDate',
    status: 'Available',
    type: 'String',
    usePreDefinedValuesOnly: false
};

await client.api('/directory/customSecurityAttributeDefinitions')
    .version('beta')
    .post(customSecurityAttributeDefinition);

```