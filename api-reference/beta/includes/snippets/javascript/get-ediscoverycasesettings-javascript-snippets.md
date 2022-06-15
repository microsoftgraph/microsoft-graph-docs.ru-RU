---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 30d2ad9e9f84eb8f49b6eb884a846ae337414dca
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094464"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryCaseSettings = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/settings')
    .version('beta')
    .get();

```