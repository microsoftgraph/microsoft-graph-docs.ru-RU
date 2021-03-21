---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1c26e0e2d63ddb8a82bcc6b41d82747e5ec4ef28
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977806"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtensionCollectionPage schemaExtensions = graphClient.schemaExtensions()
    .buildRequest()
    .filter("id eq 'graphlearn_test'")
    .get();

```