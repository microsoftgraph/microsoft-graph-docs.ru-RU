---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af591176597740220c211b93ad098551bc6d7a5e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}/participants/{id}')
    .version('beta')
    .get();

```