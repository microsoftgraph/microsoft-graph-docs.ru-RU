---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6eac2940e55a3338e7e0838307ad9f82d0bcb999
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336098"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schema schema = new Schema();
schema.baseType = "microsoft.graph.externalItem";
LinkedList<Property> propertiesList = new LinkedList<Property>();
Property properties = new Property();
properties.name = "ticketTitle";
properties.type = PropertyType.STRING;
properties.isSearchable = false;
properties.isRetrievable = false;
LinkedList<Label> labelsList = new LinkedList<Label>();
labelsList.add(Label.TITLE);
properties.labels = labelsList;
propertiesList.add(properties);
Property properties1 = new Property();
properties1.name = "priority";
properties1.type = PropertyType.STRING;
properties1.isQueryable = false;
properties1.isRetrievable = false;
properties1.isSearchable = false;
propertiesList.add(properties1);
Property properties2 = new Property();
properties2.name = "assignee";
properties2.type = PropertyType.STRING;
properties2.isRetrievable = false;
propertiesList.add(properties2);
schema.properties = propertiesList;

graphClient.external().connections("contosohr").schema()
    .buildRequest()
    .patch(schema);

```