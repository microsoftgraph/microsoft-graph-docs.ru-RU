---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bae95c94d40d6c6571c2a2bb233ef0f4f2ff7dbc22ef6e615ef9b8e3b2d64ce7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152507"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().fido2Methods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .delete();

```