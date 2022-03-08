---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8f8b1dc547292633952269a8621230ac78a641a7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339353"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let acronyms = await client.api('/search/acronyms')
    .version('beta')
    .get();

```