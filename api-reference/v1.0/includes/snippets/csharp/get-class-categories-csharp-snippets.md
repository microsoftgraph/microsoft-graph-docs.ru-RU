---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a04d6353f9768b3579dcc9a876b0d0045d2f27a3c649c4763e0812dce1b5c2d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57372391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignmentCategories = await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories
    .Request()
    .GetAsync();

```