---
title: тип ресурсов educationSubmissionResource
description: Оболочка вокруг ресурса для использования в отправке.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b24f1ea91691dd66d66848abcdb0069e9a25e4865f18f05b7682d2fb4a8f3d88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141751"
---
# <a name="educationsubmissionresource-resource-type"></a>тип ресурсов educationSubmissionResource

Пространство имен: microsoft.graph

Оболочка вокруг ресурса для использования в отправке. 

Обертка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |Чтение свойств и связей объекта **educationSubmissionResource.**|
|[Удаление](../api/educationsubmissionresource-delete.md) | Нет |Удаление **объекта educationSubmissionResource.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|Указатель на назначение, с которого был скопирован этот ресурс. Если это null, студент загрузил ресурс.|
|id|String| Только для чтения.|
|resource|[educationResource](educationresource.md)|Объект Resource.|

## <a name="relationships"></a>Связи
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


