---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a66825fd50dc6cb3b0a9e0af4fb8cdb84e038299
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookmarks = await client.api('/search/bookmarks')
    .version('beta')
    .get();

```