---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3987b77437f974f26e3e992a87a077f547206deb0c3b51b63414f8106231bdfe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57189809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScoreControlProfile = await client.api('/security/secureScoreControlProfiles/{id}')
    .get();

```