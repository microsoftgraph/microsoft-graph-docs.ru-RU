---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a89a2e254ecc923dbd1dadd1ebf640fa95cf212dfa95ca83756f65a1a291c52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extension = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral')
    .get();

```