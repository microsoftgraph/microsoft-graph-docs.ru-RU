---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bd74f315a8046c1442a0057b520186d3a22473fceb0c3224dffd84c85cba5484
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffReasons = await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .version('beta')
    .get();

```