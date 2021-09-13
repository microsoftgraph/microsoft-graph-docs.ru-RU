---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e8da0146b237f1b24c883c0bf6af19209f00eb87f916fbb793ce3743d58f8765
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57257117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationTemplate = await client.api('/applicationTemplates/{id}')
    .get();

```