---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 46c6113ad8fcad40b013f06e077623b9d248d67b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805457"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  '@odata.type': 'microsoft.graph.mailSearchFolder',
  displayName: 'Weekly digests',
  includeNestedFolders: true,
  sourceFolderIds: ['AQMkADYAAAIBDAAAAA=='],
  filterQuery: 'contains(subject, \'weekly digest\')'
};

await client.api('/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders')
    .version('beta')
    .post(mailFolder);

```