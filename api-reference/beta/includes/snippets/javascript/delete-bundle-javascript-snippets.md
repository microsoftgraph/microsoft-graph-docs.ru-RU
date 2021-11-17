---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b67c23eee5bc9f6a79d81754a4cc508dcdafa7a153a192dd8cbc63c5bf9c676f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .delete();

```