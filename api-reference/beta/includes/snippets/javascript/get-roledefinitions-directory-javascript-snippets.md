---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f38b50779bd0d984ce6f05cf94ff5f9600d73569
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869169"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleDefinitions = await client.api('/roleManagement/directory/roleDefinitions')
    .version('beta')
    .get();

```