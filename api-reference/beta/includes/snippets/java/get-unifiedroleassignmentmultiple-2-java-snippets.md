---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 25264f3f9c48d21b3d23a4be950bf835cd31af66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960633"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUnifiedRoleAssignmentMultipleCollectionPage roleAssignments = graphClient.roleManagement().deviceManagement().roleAssignments()
    .buildRequest()
    .get();

```