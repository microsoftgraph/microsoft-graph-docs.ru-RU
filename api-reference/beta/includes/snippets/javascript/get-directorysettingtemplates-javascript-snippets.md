---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 85cfa0ca3c0713b8b4255ba0e0124c2ef582b9bc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810072"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directorySettingTemplates = await client.api('/directorySettingTemplates')
    .version('beta')
    .get();

```