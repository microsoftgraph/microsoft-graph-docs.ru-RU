---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a8938cf25a70e0dda1c3990e618ca2561f529cd0f0effce2be2d3dbb030c33a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57324709"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let relations = await client.api('/termStore/sets/{setId}/relations')
    .version('beta')
    .get();

```