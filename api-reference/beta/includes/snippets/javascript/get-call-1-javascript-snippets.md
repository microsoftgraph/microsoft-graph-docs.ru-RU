---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 42a6db6c17afa3c8e7dddf0e22822c2008cfd3e6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let call = await client.api('/communications/calls/{id}')
    .version('beta')
    .get();

```