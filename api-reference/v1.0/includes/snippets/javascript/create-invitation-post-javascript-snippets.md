---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f565f403d89b233c8556b426ad316532e721865b
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const invitation = {
  invitedUserEmailAddress: "yyy@test.com",
  inviteRedirectUrl: "https://myapp.contoso.com"
};

let res = await client.api('/invitations')
    .post(invitation);

```