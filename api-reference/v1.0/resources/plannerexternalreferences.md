---
title: тип ресурса plannerExternalReferences
description: Ресурс **plannerExternalReferences** представляет коллекцию ссылок на задачу. Это открытый тип. Это часть объекта сведений о задачах. Значение в паре свойство-значение — объект externalReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6a82c13a4fd18c66be3b6d2c0e8753f9fefd1ab6fdc0c47ac305ef34ff6acfba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237546"
---
# <a name="plannerexternalreferences-resource-type"></a>тип ресурса plannerExternalReferences

Пространство имен: microsoft.graph

Ресурс **plannerExternalReferences** представляет коллекцию ссылок на задачу. Это открытый тип. Это часть объекта [сведений о задачах.](plannertaskdetails.md) Значение в паре свойство-значение — [объект externalReference.](plannerexternalreference.md)


## <a name="properties"></a>Свойства
Свойства открытого типа могут быть определены клиентом. В этом случае клиент должен предоставить допустимые **URL-адреса** на основе протоколов **HTTP/HTTPS,** так как свойствами и их значениями должны быть [объекты externalReference.](plannerexternalreference.md) На основе OData имена свойств в Open Types не могут содержать следующие символы: , , , поэтому они `.` `:` должны быть `%` `@` `#` закодированы. Пример показан ниже. Чтобы удалить ссылку, установите значение свойства `null` .

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerExternalReferences"
}-->


```json
{
  "String-value":
  {
    "alias": "String-value",
    "lastModifiedBy": "String-value",
    "lastModifiedDateTime": "String(timestamp)",
    "previewPriority": "String-value",
    "type": "String-value"
  }
}
```

## <a name="example"></a>Пример

```json
{
  "https%3A//contoso%2Esharepoint%2Ecom/teams/agile/documents/AnnualReport%2Epptx":
  {
    "@odata.type": "microsoft.graph.externalReference", // required in PATCH requests to edit the references on a task
    "alias": "Agile Team Annual Report",
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedDateTime": "2015-09-21T17:45:12.039Z",
    "previewPriority": "0009005756397228702",
    "type": "PowerPoint"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

