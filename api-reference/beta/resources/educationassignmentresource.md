---
title: Тип ресурса Едукатионассигнментресаурце
description: Объект-оболочка, в котором хранятся ресурсы, связанные с назначением. Упаковщик добавляет свойство **дистрибутефорстудентворк** и указывает на то, что этот ресурс
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60181a2289b272809cff025abeee83c594ae833e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006432"
---
# <a name="educationassignmentresource-resource-type"></a>Тип ресурса Едукатионассигнментресаурце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект-оболочка, в котором хранятся ресурсы, связанные с назначением. Оболочка добавляет свойство **дистрибутефорстудентворк** и указывает, что этот ресурс будет скопирован в отправку учащегося.  Если объект не копируется, каждый учащийся увидит ссылку на ресурс на назначении. Учащийся не сможет обновить этот ресурс. Это выдача от преподавателя к студенту, которую не следует включать. Если ресурс распространяется, каждый учащийся получит копию этого ресурса в списке ресурсов их отправки. Каждый студент сможет изменить свою копию и отправит их для ступенчатого.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Едукатионассигнментресаурце](../api/educationassignmentresource-get.md) | [Едукатионассигнментресаурце](educationassignmentresource.md) |Чтение свойств и связей объекта **едукатионассигнментресаурце** .|
|[обновление](../api/educationassignmentresource-update.md); | [Едукатионассигнментресаурце](educationassignmentresource.md) |Обновление объекта **едукатионассигнментресаурце** . |
|[Удаление](../api/educationassignmentresource-delete.md) | Нет |Удаление объекта **едукатионассигнментресаурце** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Дистрибутефорстудентворк|Boolean|Указывает, следует ли копировать этот ресурс в каждую отправку учащегося для изменения и отправки.|
|id|String| ИДЕНТИФИКАТОР этого ресурса. Только для чтения.|
|resource|[Едукатионресаурце](educationresource.md)|Объект ресурса, связанный с этим назначением.|

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
