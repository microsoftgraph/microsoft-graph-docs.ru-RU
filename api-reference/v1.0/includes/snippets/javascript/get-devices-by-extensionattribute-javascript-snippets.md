---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d607778a0c2430dd76cac3d55a0ac4f186d5f8c
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694845"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/devices')
    .header('ConsistencyLevel','eventual')
    .filter('extensionAttributes/extensionAttribute1 eq \'BYOD-Device\'')
    .get();

```