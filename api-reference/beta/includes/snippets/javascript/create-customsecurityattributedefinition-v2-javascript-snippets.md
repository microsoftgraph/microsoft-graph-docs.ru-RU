---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f88a6ffcc462f00954cf47b3126fe5ebf4528951
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const customSecurityAttributeDefinition = {
    attributeSet: 'Engineering',
    description: 'Active projects for user',
    isCollection: true,
    isSearchable: true,
    name: 'Project',
    status: 'Available',
    type: 'String',
    usePreDefinedValuesOnly: true
};

await client.api('/directory/customSecurityAttributeDefinitions')
    .version('beta')
    .post(customSecurityAttributeDefinition);

```