---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8fb42e7ecd09c607e278140401980582ac8b1bab
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60561971"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentResource = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources/a2f95693-aea2-4d5e-a936-11ef390f8f20')
    .version('beta')
    .get();

```