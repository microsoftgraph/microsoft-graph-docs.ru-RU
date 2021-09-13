---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 09c8543ac07d073b67ee52317e00f180cea51271521121baab742ae024dadd86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/groups/{groupId}/drive')
    .get();

```