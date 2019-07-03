---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e1836c0075f3a7c3e0d6b026480ca15348cc65c2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529923"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateProperties = {
  entityType: "Group",
  displayName: "Myprefix_test_mysuffix",
  mailNickname: "Myprefix_test_mysuffix",
  onBehalfOfUserId: "onBehalfOfUserId-value"
};

let res = await client.api('/directoryObjects/validateProperties')
    .version('beta')
    .post(validateProperties);

```