---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3859e2648aefcd54cf5400b8f2869ee0e302805f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920174"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xUserFlows = await client.api('/identity/b2xUserFlows')
    .get();

```