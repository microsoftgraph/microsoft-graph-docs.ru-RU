---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 91813d5dbe83e56afe364199ef7872f87e6f605f
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/organization/99b24e1b-abec-4598-9d63-a2baf0a3cea1/branding/localizations/fr-FR/signInPageText')
    .get();

```