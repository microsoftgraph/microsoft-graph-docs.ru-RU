---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14cdea444c2da29042e253b5f9f751ed18ac5975
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schemaExtension = await client.api('/schemaExtensions/graphlearn_test')
    .get();

```