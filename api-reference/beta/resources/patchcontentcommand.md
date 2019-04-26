---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
ms.openlocfilehash: d0d8f320d22a8b3466ddd53deee5bcb7955ff3d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568481"
---
# <a name="patchcontentcommand-resource-type"></a>Тип ресурса Патчконтенткомманд

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.

## <a name="json-representation"></a>Описание в формате JSON

Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [Patch Pages/{ID} '](../api/page-update.md) . 

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
|action|String|Действие, которое необходимо выполнить для целевого элемента. Возможные значения: `replace`, `append`, `delete`, `insert` и `prepend`.|
|content|String|Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла. Если содержимое содержит двоичные данные, необходимо отправить запрос, используя тип `multipart/form-data` контента с частью "Commands". |
|position|String|Место для добавления предоставленного контента относительно целевого элемента. Возможные значения: `after` (по умолчанию) `before`или.|
|target|String|Обновляемый элемент. Должен быть `#<data-id>` либо сгенерированным `<id>` элементом, либо ключевым словом `body` or. `title`|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/patchcontentcommand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
