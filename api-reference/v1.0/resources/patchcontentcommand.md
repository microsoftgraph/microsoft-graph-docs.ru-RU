---
title: Тип ресурса patchContentCommand
description: Изменения, внося в OneNote в запросе PATCH.
ms.localizationpriority: medium
author: jewan-microsoft
ms.prod: notes
doc_type: resourcePageType
ms.openlocfilehash: b5432bf68cfc4acdc42db0c502555469ca025d71
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034686"
---
# <a name="patchcontentcommand-resource-type"></a>Тип ресурса patchContentCommand

Пространство имен: microsoft.graph

Изменения, внося в OneNote в запросе PATCH.

## <a name="json-representation"></a>Представление JSON

Ниже приведено представление ресурса в формате JSON, которое отправляется в тексте запроса [PATCH pages/{id}](../api/page-update.md) .

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
|action|onenotePatchActionType|Действие, выполняемые с целевым элементом. Возможные значения: `replace`, , `append`, `delete`, или `insert``prepend`.|
|content|String|Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла. Если содержимое содержит двоичные данные, запрос `multipart/form-data` должен быть отправлен с использованием типа контента с частью "Команды". |
|position|OnenotePatchInsertPosition|Место для добавления предоставленного контента относительно целевого элемента. Возможные значения: `after` (по умолчанию) или `before`.|
|target|Строка|Обновляемый элемент. Должен быть либо `#<data-id>` созданным `<id>` элементом, либо ключевым словом `body` `title` .|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

