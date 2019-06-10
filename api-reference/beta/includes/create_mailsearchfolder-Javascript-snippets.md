---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3e88b0a99d983d2ed741cc1bac73716f4787ba61
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  @odata.type: "microsoft.graph.mailSearchFolder",
  displayName: "Get MyAnalytics",
  includeNestedFolders: true,
  sourceFolderIds: ["AAMkAGVmMDEzM"],
  filterQuery: "contains(subject, 'MyAnalytics')"
};

let res = await client.api('/me/mailFolders/searchfolders/childfolders')
    .version('beta')
    .post({mailFolder : mailFolder});

```