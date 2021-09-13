---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e3d6133d070cff93596ae1fd762cdbae47ea292bbf8cc1599920b37312624c73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57366954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/acceptedSenders/$ref')
    .delete();

```