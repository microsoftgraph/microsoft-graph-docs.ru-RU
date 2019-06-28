---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b0897fe2ba6b22fad7f0bf1febf8ad51c86fffe6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35326450"
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
    .post({mailFolder : mailFolder});

```