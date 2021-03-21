---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4b240b40f0e9952e61e9b644fceb9fe6757d36f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981029"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtension schemaExtension = new SchemaExtension();
LinkedList<ExtensionSchemaProperty> propertiesList = new LinkedList<ExtensionSchemaProperty>();
ExtensionSchemaProperty properties = new ExtensionSchemaProperty();
properties.name = "new-name-value";
properties.type = "new-type-value";
propertiesList.add(properties);
ExtensionSchemaProperty properties1 = new ExtensionSchemaProperty();
properties1.name = "additional-name-value";
properties1.type = "additional-type-value";
propertiesList.add(properties1);
schemaExtension.properties = propertiesList;

graphClient.schemaExtensions("{id}")
    .buildRequest()
    .patch(schemaExtension);

```