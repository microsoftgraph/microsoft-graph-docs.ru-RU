---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9bfd6cb1dc407c2c8d28b856a98fbb1af6ea1e73
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60561430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSubmissionResource = await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources/31f2c67a-6df1-4a7f-b4c5-311fe15c873a')
    .version('beta')
    .get();

```