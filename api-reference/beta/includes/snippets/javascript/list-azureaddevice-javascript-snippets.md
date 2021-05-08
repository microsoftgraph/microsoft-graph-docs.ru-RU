---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb1451372a6195f2660fa334e9a8162e9e86ae62
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let updatableAssets = await client.api('/admin/windows/updates/updatableAssets/')
    .version('beta')
    .filter('isof(\'microsoft.graph.windowsUpdates.azureADDevice\')')
    .get();

```