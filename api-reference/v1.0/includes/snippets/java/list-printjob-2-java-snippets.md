---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e778b53cb14ebb5b0fa845b49178aeb1c5a2807a3c95c85b60ff42b3999cdf5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57205200"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobCollectionPage jobs = graphClient.print().shares("{printerShareId}").jobs()
    .buildRequest()
    .get();

```