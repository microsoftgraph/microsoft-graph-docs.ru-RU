---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8e314ab118fd0529c826c6afb0a30e55930d147b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowLanguageConfiguration = await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en')
    .get();

```