---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
ms.openlocfilehash: 79a01c59ec0a891c13107095a950a7cc8ae0b547
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074877"
---
# <a name="mailboxsettings-resource-type"></a>Тип ресурса mailboxSettings

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Параметры основного параметра вошедшего пользователя.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|archiveFolder|string|Идентификатор архивной папки пользователя.|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.|
|language|[localeInfo](localeinfo.md)|Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.|
|timeZone|string|Часовой пояс почтового ящика пользователя по умолчанию.|
|workingHours|[workingHours](workinghours.md)|Дни недели и часы работы пользователя в определенном часовом поясе.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->