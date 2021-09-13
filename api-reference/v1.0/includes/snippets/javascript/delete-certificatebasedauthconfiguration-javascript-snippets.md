---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc3e1cef1da3b8ced48769c48e7f2b526ffa07154a271ba356654b7f14906894
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57312030"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .delete();

```