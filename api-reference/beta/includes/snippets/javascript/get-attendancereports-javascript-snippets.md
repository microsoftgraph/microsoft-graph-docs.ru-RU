---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bab6d7b8690c84df821f8c1949a15805bf83741b
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225332"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attendanceReports = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports')
    .version('beta')
    .get();

```