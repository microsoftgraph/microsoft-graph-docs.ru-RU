---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 240b89e018b81cfa97ec6ca47ea93b321b5ca90b6203659ff0a804bfcf228872
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57195345"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tag = {
  description: 'This is an updated description.'
};

await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504')
    .version('beta')
    .update(tag);

```