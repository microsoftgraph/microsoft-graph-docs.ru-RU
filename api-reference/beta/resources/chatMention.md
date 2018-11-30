---
title: Тип ресурса chatMessageMention
description: 'Представляет упоминаются в сущности chatMessage. Упоминание может быть пользователь, группа, программа-робот или канала. '
ms.openlocfilehash: 5f1e427b0ed2b8ffcfbc86417beb4719dc6fb2a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075099"
---
# <a name="chatmessagemention-resource-type"></a>Тип ресурса chatMessageMention

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет упоминаются в сущности [chatMessage](chatmessage.md) . Упоминание может быть пользователь, группа, программа-робот или канала. 

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка|Идентификатор сущности упоминаемые|
|mentionText|string|Строка, используемая для представления упоминание Ex: отображаемое имя пользователя, имя группы и т.д.|
|упомянутые|[identitySet](identityset.md)|Пользователь, который был упомянут|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
