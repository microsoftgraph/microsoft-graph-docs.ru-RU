---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 113e3be4de933442bb07796cc634107118f079eb
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityUserFlowAttribute = await client.api('/identity/userFlowAttributes/{id}')
    .get();

```