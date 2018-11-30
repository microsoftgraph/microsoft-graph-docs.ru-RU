---
title: Тип ресурса patchContentCommand
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
ms.openlocfilehash: bfbdceeda0294540f701f9fa458030834e7d7850
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025446"
---
# <a name="patchcontentcommand-resource-type"></a>Тип ресурса patchContentCommand

Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [PATCH pages/{id}`](../api/page-update.md). 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|action|onenotePatchActionType|Действие, которое требуется выполнить с целевым элементом. Возможные значения: `replace`, `append`, `delete`, `insert`, или `prepend`.|
|content|String|Строка правильно оформленного HTML-кода, который необходимо добавить на страницу, а также двоичные данные любого изображения или файла. Если контент содержит двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands. |
|position|onenotePatchInsertPosition|Расположение относительно целевого элемента, куда нужно добавить указанное содержимое. Возможные значения: `after` (по умолчанию) или `before`.|
|target|String|Элемент для обновления. Значение этого свойства должно представлять собой `#<data-id>`, созданный идентификатор `<id>` элемента либо ключевое слово `body` или `title`.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
