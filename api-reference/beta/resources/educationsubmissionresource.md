---
title: Тип ресурса Едукатионсубмиссионресаурце
description: 'Оболочка для ресурса, используемая при отправке. Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b96607a0d37a3ec8af0f6ff0bad61215d6e9008c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340597"
---
# <a name="educationsubmissionresource-resource-type"></a>Тип ресурса Едукатионсубмиссионресаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Оболочка для ресурса, используемая при отправке. Оболочка добавляет указатель на ресурс назначения, если он был скопирован из назначения.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Едукатионсубмиссионресаурце](../api/educationsubmissionresource-get.md) | [Едукатионсубмиссионресаурце](educationsubmissionresource.md) |Чтение свойств и связей объекта **едукатионсубмиссионресаурце** .|
|[Delete](../api/educationsubmissionresource-delete.md) | Нет |Удаление объекта **едукатионсубмиссионресаурце** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Ассигнментресаурцеурл|String|Указатель на назначение, из которого был скопирован данный ресурс. Если это значение равно null, учащийся передал ресурс.|
|id|String| Только для чтения.|
|resource|[Едукатионресаурце](educationresource.md)|Объект Resource.|

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
