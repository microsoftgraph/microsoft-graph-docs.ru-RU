---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5da5e2294845fdf0aba2029acd410a59a7c0806c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135232"
---
# <a name="mailboxsettings-resource-type"></a>Тип ресурса mailboxSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры основного почтового ящика [пользователя.](user.md)

Вы можете [получить](../api/user-get-mailboxsettings.md) или [обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросив свойство **mailboxSettings пользователя.**


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|archiveFolder|string|Идентификатор архивной папки пользователя. Только для чтения.|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.|
|dateFormat|string|Формат даты для почтового ящика пользователя.|
|delegateMeetingMessageDeliveryOptions|delegateMeetingMessageDeliveryOptions| Если у пользователя есть делегат календаря, это указывает, будет ли делегат, владелец почтового ящика или оба получать сообщения о собрании и ответы на них. Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`. Значение по `sendToDelegateOnly` умолчанию: .|
|language|[localeInfo](localeinfo.md)|Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.|
|timeFormat|string|Формат времени для почтового ящика пользователя.|
|timeZone|string|Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.|
|workingHours|[workingHours](workinghours.md)|Дни недели и часы работы пользователя в определенном часовом поясе.|
|userPurpose|[userPurpose](userpurpose.md)|Назначение почтового ящика. Используется для различения почтового ящика отдельного пользователя от общего почтового ящика и почтового ящика оборудования в Exchange Online. Только для чтения.|

## <a name="json-representation"></a>Представление в формате JSON

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
  "dateFormat": "string",
  "delegateMeetingMessageDeliveryOptions": "String",
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeFormat": "string",
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"},
  "userPurpose": {"@odata.type": "microsoft.graph.userPurpose"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


