---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d113966562164712361e2f9e1c13d28b1ec1047
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513628"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSettingTemplate = await client.api('/groupSettingTemplates/08d542b9-071f-4e16-94b0-74abb372e3d9')
    .get();

```