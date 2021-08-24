---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07443842a9ae09b84b168e401f3ac3b806927e783a4851b7df989cc3e898d6a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57325528"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupSettings = await client.api('/groupSettings')
    .get();

```