---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 862f9153f2f5b54a11f248ad40c8baf0132c9d5f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  @odata.type: "microsoft.graph.mailSearchFolder",
  displayName: "Weekly digests",
  includeNestedFolders: true,
  sourceFolderIds: ["AQMkADYAAAIBDAAAAA=="],
  filterQuery: "contains(subject, 'weekly digest')"
};

let res = await client.api('/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders')
    .version('beta')
    .post({mailFolder : mailFolder});

```