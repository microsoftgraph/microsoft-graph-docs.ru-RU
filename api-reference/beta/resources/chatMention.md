---
title: Тип ресурса chatMessageMention
description: 'Представляет упоминаются в сущности chatMessage. Упоминание может быть пользователь, группа, программа-робот или канала. '
localization_priority: Normal
ms.openlocfilehash: 7b24d2af6f61f3da69480557e1c5b5f32c009c25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876141"
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
