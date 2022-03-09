---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4f12dbd45e50cb523309b63e990e3f1ab987aad3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contactMergeSuggestions = await client.api('/me/settings/contactMergeSuggestions')
    .version('beta')
    .get();

```