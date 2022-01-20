---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0da6dd42d29a16eda37b324eeaca1fd2e2158b2f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101817"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attendanceRecords = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports/c9b6db1c-d5eb-427d-a5c0-20088d9b22d7/attendanceRecords')
    .get();

```