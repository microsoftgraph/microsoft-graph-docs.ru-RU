---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: da313bb9484a80599cfb65e3dcf554c7c33281a7c17214220be67ca557a1bb07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeMembers = {
  assets: [
    {
      '@odata.type': '#microsoft.graph.windowsUpdates.azureADDevice',
      id: 'String (identifier)'
    }
  ]
};

await client.api('/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers')
    .version('beta')
    .post(removeMembers);

```