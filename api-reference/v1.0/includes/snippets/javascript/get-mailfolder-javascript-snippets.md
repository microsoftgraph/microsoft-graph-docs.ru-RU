---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3e70cdb2696c7c535bbd0e8853f6835cc68450512dc607418cf968999009ceeb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57365775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolder = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .get();

```