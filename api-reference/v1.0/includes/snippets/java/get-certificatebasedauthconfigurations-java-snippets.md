---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b5bebd0892723b8fea830a405efb125df57ef4285420073e9b223e25dcc599c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57323214"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CertificateBasedAuthConfigurationCollectionWithReferencesPage certificateBasedAuthConfiguration = graphClient.organization("{id}").certificateBasedAuthConfiguration()
    .buildRequest()
    .get();

```