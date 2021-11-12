---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3dd8b63118964b85f75e458a22fd87db75a87f8ad60863953550bc553846d101
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskTriggers = await client.api('/print/printers/{printerId}/taskTriggers')
    .get();

```