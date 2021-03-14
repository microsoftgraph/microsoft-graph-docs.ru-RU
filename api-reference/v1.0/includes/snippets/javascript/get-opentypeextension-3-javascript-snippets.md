---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 67ada1c367d8ea7cc0ea4a97a7a12a6d6ebe1dc1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809114"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')
    .expand('extensions($filter=id%20eq%20\'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral\')')
    .get();

```