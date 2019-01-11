---
title: Тип ресурса plannerExternalReferences
description: Ресурс **plannerExternalReferences** представляет коллекцию справочных материалов для задачи. Это открытый тип. Он является частью объекта сведений о задаче. Значение в паре "свойство-значение" представляет собой объект externalReference.
localization_priority: Normal
ms.openlocfilehash: aedfd0321843c4a906defe22f184bac7d293a6e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862078"
---
# <a name="plannerexternalreferences-resource-type"></a>Тип ресурса plannerExternalReferences

Ресурс **plannerExternalReferences** представляет коллекцию справочных материалов для задачи. Это открытый тип. Он является частью объекта [сведений о задаче](plannertaskdetails.md). Значение в паре "свойство-значение" представляет собой объект [externalReference](plannerexternalreference.md).


## <a name="properties"></a>Свойства
Клиент может определять свойства открытого типа. В этом случае клиент должен предоставить **допустимые URL-адреса** на базе протоколов **HTTP/HTTPS** в качестве свойств с объектами [externalReference](plannerexternalreference.md) в качестве значений. Согласно OData имена свойств в открытых типах не могут содержать символы `.`, `:` и `%`, поэтому их нужно зашифровать. Ниже показан пример. Чтобы удалить определенные справочные материалы, задайте свойству значение `null`.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

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

Пример:

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
