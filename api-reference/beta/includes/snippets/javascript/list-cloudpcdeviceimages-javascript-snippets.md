---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 640295402568add90933903f3252f97d53e499c7891f1d802b0c295607e1f4b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deviceImages = await client.api('/deviceManagement/virtualEndpoint/deviceImages')
    .version('beta')
    .get();

```