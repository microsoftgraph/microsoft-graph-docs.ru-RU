---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc5e991e435d6474b79bfc71fccf7825f4b54272
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 '@odata.id':'https://graph.microsoft.com/v1.0/education/classes/11006'
};

await client.api('/education/schools/{school-id}/classes/$ref')
    .post(educationClass);

```