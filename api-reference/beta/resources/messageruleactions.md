---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 58cae7f777d0ac9ee03b102b22325e63acf55358
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938890"
---
# <a name="messageruleactions-resource-type"></a>Тип ресурса messageRuleActions

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет набор действий, доступных для правила.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| assignCategories | Коллекция String | Список категорий, которые необходимо назначить сообщению. |
| copyToFolder | String | Идентификатор папки, в которую необходимо скопировать сообщение. |
| delete | Boolean | Указывает, нужно ли перемещать сообщение в папку "Удаленные". |
| forwardAsAttachmentTo | Коллекция [recipient](recipient.md) | Электронные адреса получателей, которым необходимо переслать сообщение как вложение. |
| forwardTo | Коллекция [recipient](recipient.md) | Электронные адреса получателей, которым необходимо переслать сообщение. |
| markAsRead | Boolean | Указывает, необходимо ли отмечать сообщение как прочтенное. |
| markImportance | String | Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`. |
| moveToFolder |  String| Идентификатор папки, в которую сообщение будет перемещено. |
| permanentDelete | Boolean | Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные". |
| redirectTo | [recipient](recipient.md) | Электронный адрес, на который должно быть перенаправлено сообщение. |
| stopProcessingRules | Boolean | Указывает, должны ли обрабатываться последующие правила. |


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
