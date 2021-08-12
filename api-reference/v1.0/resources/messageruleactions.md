---
title: Тип ресурса messageRuleActions
description: Представляет набор действий, доступных для правила.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 96e6005a4297eafc1cf5905d9ad0b60c3c43bfeef496fa529bf6261d7233dd0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235403"
---
# <a name="messageruleactions-resource-type"></a>Тип ресурса messageRuleActions

Пространство имен: microsoft.graph


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
| markImportance | importance | Задает важность сообщения. Допустимые значения: `low`, `normal`, `high`. |
| moveToFolder |  String| Идентификатор папки, в которую сообщение будет перемещено. |
| permanentDelete | Boolean | Указывает, нужно ли окончательно удалять сообщение без сохранения в папке "Удаленные". |
| redirectTo | Коллекция [recipient](recipient.md) | Адреса электронной почты, на которые должно быть перенаправлено сообщение. |
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
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
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

