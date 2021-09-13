---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a6084c3b0bd2ec719cf2aa742f247ee130ff80c32b59dfd98670aa61b0141f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57270916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sharedWithMe = await client.api('/me/drive/sharedWithMe')
    .get();

```