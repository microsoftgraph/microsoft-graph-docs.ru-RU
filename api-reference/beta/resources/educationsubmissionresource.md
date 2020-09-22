---
title: Тип ресурса Едукатионсубмиссионресаурце
description: 'Оболочка для ресурса, используемая при отправке. Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 329bab18d90412ec8cc06b12106e0be4f1b46935
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979569"
---
# <a name="educationsubmissionresource-resource-type"></a>Тип ресурса Едукатионсубмиссионресаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Оболочка для ресурса, используемая при отправке. Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Едукатионсубмиссионресаурце](../api/educationsubmissionresource-get.md) | [едукатионсубмиссионресаурце](educationsubmissionresource.md) |Чтение свойств и связей объекта **едукатионсубмиссионресаурце** .|
|[удаление](../api/educationsubmissionresource-delete.md); | Нет |Удаление объекта **едукатионсубмиссионресаурце** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ассигнментресаурцеурл|String|Указатель на назначение, из которого был скопирован данный ресурс. Если это значение равно null, учащийся передал ресурс.|
|id|String| Только для чтения.|
|resource|[едукатионресаурце](educationresource.md)|Объект Resource.|

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


