---
title: Тип ресурса Планнерекстерналреференцес
description: Ресурс **планнерекстерналреференцес** представляет коллекцию ссылок на задачу. Это открытый тип. Он является частью объекта сведений о задаче. Значение в параметре "свойство-значение" является объектом Екстерналреференце.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5c67aadd421d4f7ac3ac96527dc85deef33de722
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330335"
---
# <a name="plannerexternalreferences-resource-type"></a>Тип ресурса Планнерекстерналреференцес

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **планнерекстерналреференцес** представляет коллекцию ссылок на задачу. Это открытый тип. Он является частью объекта [сведений о задаче](plannertaskdetails.md) . Значение в параметре "свойство-значение" является объектом [екстерналреференце](plannerexternalreference.md) .


## <a name="properties"></a>Свойства
Клиентская возможность может определять свойства открытого типа. В этом случае клиент должен предоставить **действительные URL-адреса** на основе протоколов **HTTP/HTTPS** , а их значения должны быть объектами [екстерналреференце](plannerexternalreference.md) . На основе OData имена свойств в открытых типах не могут содержать следующие символы: `.` , `:` и `%`  поэтому их необходимо закодировать. Пример показан ниже. Чтобы удалить ссылку, присвойте свойству значение `null` .

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


