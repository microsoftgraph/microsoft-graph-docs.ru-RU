---
title: тип ресурса patchContentCommand
description: Изменения, внесенные на страницу OneNote в запросе PATCH.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0b34271f08cc8f8e234c6a10ecd28229ddbce451ca0f54b26197bc1a9d02f56f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205257"
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
|target|String|Обновляемый элемент. Должен быть `#<data-id>` или созданный `<id>` элемент, или ключевое `body` слово или `title` ключевое слово.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

