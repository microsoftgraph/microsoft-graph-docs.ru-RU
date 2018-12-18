---
title: Тип ресурса educationSubmissionResource
description: 'Оболочку ресурсов для использования на отправку. Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.  '
author: dipakboyed
ms.openlocfilehash: bfbf2f522106f5a1e2033898cbb2702223d3e241
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361560"
---
# <a name="educationsubmissionresource-resource-type"></a>Тип ресурса educationSubmissionResource

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Оболочку ресурсов для использования на отправку. Программа-оболочка добавляет указатель назначения ресурсов в том случае, если это скопированный из назначения.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |Чтение свойства и связи объекта **educationSubmissionResource** .|
|[Delete](../api/educationsubmissionresource-delete.md) | Нет |Удаление объекта **educationSubmissionResource** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String.|Указатель на назначения, с которого был скопирован этот ресурс. Если это значение null, студент загружаться ресурса.|
|id|Строка| Только для чтения.|
|resource|[educationResource](educationresource.md)|Объект ресурса.|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->