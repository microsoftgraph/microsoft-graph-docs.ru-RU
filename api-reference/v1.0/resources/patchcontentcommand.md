---
title: тип ресурса patchContentCommand
description: Изменения, внесенные на страницу OneNote в запросе PATCH.
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 633bd39ec3bb3a95c9c2c9ba5755baf5e04dd298
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117931"
---
# <a name="patchcontentcommand-resource-type"></a>тип ресурса patchContentCommand

Пространство имен: microsoft.graph

Изменения, внесенные на страницу OneNote в запросе PATCH.

## <a name="json-representation"></a>Представление JSON

Вот представление JSON ресурса, которое отправляется в тело страницы [PATCH/{id}'](../api/page-update.md) запроса.

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
|action|onenotePatchActionType|Действие для выполнения на целевом элементе. Возможные значения: `replace` `append` , , , , `delete` или `insert` `prepend` .|
|content|String|Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла. Если содержимое содержит двоичные данные, запрос должен быть отправлен с помощью типа контента с частью `multipart/form-data` "Команды". |
|position|onenotePatchInsertPosition|Место для добавления предоставленного контента относительно целевого элемента. Возможные значения: `after` (по умолчанию) или `before` .|
|target|Строка|Обновляемый элемент. Должен быть `#<data-id>` или созданный `<id>` элемент, или ключевое `body` слово или `title` ключевое слово.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

