---
title: тип ресурсов educationSubmissionResource
description: Оболочка вокруг ресурса для использования в отправке.
author: sharad-sharma-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 632e2d746e4204e2c3c64f429f443ff40ed5a69f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118738"
---
# <a name="educationsubmissionresource-resource-type"></a>тип ресурсов educationSubmissionResource

Пространство имен: microsoft.graph

Оболочка вокруг ресурса для использования в отправке. 

Обертка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |Чтение свойств и связей объекта **educationSubmissionResource.**|
|[удаление](../api/educationsubmissionresource-delete.md); | Нет |Удаление **объекта educationSubmissionResource.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignmentResourceUrl|Строка|Указатель на назначение, с которого был скопирован этот ресурс. Если это null, студент загрузил ресурс.|
|id|String| Только для чтения.|
|resource|[educationResource](educationresource.md)|Объект Resource.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


