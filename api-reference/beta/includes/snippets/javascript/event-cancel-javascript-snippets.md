---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49a6d00bb09c5c248744b7e1162bd55ad18059c03f9c53b79e3988f9f1838986
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143528"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  Comment: 'Cancelling for this week due to all hands'
};

await client.api('/me/events/{id}/cancel')
    .version('beta')
    .post(cancel);

```