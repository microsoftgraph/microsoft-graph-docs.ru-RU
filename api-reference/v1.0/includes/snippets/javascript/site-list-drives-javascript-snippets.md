---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e7286368f934f83fc95de9779e4f44e876abc4ebaa977c07d753275d261c3f38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57203678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/sites/{siteId}/drives')
    .get();

```