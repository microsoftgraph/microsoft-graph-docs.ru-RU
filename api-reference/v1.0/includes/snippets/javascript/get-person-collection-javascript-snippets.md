---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a70f1b99cd524d8d74f629259d793b1bad67fc22434060a2d5102734f020ca9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57253760"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let people = await client.api('/me/people')
    .get();

```