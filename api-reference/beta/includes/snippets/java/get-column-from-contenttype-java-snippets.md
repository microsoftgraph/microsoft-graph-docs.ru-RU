---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2b2b9d01175dd82c768537bd27eb79a2862310987b21d47b359f52658bed3dff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144607"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinition columnDefinition = graphClient.sites("{site-id}").contentTypes("{contentType-id}").columns("{column-id}")
    .buildRequest()
    .get();

```