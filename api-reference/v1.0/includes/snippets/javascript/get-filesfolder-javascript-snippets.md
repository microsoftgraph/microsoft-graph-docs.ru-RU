---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: edca17b2901ff408d412f0721b11eb426d455d70
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863427"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}/filesFolder')
    .get();

```