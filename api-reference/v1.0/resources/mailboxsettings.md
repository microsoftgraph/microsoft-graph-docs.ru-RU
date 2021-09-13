---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4a6e053e60616464c8d1f3facc5394398a2346e5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089335"
---
# <a name="mailboxsettings-resource-type"></a>Тип ресурса mailboxSettings

Пространство имен: microsoft.graph

Параметры для основного почтового ящика [пользователя](user.md).

Вы можете [получить](../api/user-get-mailboxsettings.md) или [обновить](../api/user-update-mailboxsettings.md) параметры почтовых ящиков пользователя, запросив свойство **mailboxSettings** пользователя.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|archiveFolder|string|Идентификатор архивной папки пользователя.|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.|
|dateFormat|string|Формат даты для почтового ящика пользователя.|
|delegateMeetingMessageDeliveryOptions|delegateMeetingMessageDeliveryOptions| Если у пользователя есть делегат календаря, это указывает, получает ли делегат, владелец почтового ящика или как получать сообщения о собраниях, так и ответы на собрания. Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.|
|language|[localeInfo](localeinfo.md)|Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.|
|timeFormat|string|Формат времени для почтового ящика пользователя.|
|timeZone|string|Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.|
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
  "dateFormat": "string",
  "delegateMeetingMessageDeliveryOptions": "String",
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeFormat": "string",
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

