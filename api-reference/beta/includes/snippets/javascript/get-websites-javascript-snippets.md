---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a21095b47db6b4a2ae0d894cdb4a43aeef9aeffbf8ca4b649ba75b8b8928cbde
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252629"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let websites = await client.api('/me/profile/websites')
    .version('beta')
    .get();

```