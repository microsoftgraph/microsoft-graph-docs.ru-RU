---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81354489104f71490f739c4b7262f059ff49e12b4ed3084d5b5dedf578ba03fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57270928"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveSharedWithMeCollectionPage sharedWithMe = graphClient.me().drive()
    .sharedWithMe()
    .buildRequest()
    .get();

```