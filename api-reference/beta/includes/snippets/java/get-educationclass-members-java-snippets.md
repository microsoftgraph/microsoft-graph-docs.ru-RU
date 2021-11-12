---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4843df3c9d8a12351220ce7b774075fa03df8eebc99a9e1472a01035b030f14e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144268"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage members = graphClient.education().classes("11016").members()
    .buildRequest()
    .get();

```