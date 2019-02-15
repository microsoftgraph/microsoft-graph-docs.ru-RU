---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Normal
ms.openlocfilehash: ee5359c0ababad2a4f785d17a02ac5bb618d2681
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057045"
---
# <a name="datetimetimezone-resource-type"></a>Тип ресурса dateTimeTimeZone

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает дату, время и часовой пояс для определенного момента.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|dateTime|String|Один момент времени в объединенном представлении даты и времени (`{date}T{time}`). Пример: "2019 – 04 – 16T09:00:00".|
|timeZone|String|Название часового пояса, как описано ниже.|

Для свойства **TimeZone** можно задать любой часовой пояс, поддерживаемый Windows, а также следующие имена часовых поясов.

Etc/GMT+12

Etc/GMT+11

Pacific/Honolulu

America/Anchorage

America/Santa_Isabel

America/Los_Angeles

America/Phoenix

America/Chihuahua

America/Denver

America/Guatemala

America/Chicago

America/Mexico_City

America/Regina

America/Bogota

America/New_York

America/Indiana/Indianapolis

America/Caracas

America/Asuncion

America/Halifax

America/Cuiaba

America/La_Paz

America/Santiago

America/St_Johns

America/Sao_Paulo

America/Argentina/Buenos_Aires

America/Cayenne

America/Godthab

America/Montevideo

America/Bahia

Etc/GMT+2

Atlantic/Azores

Atlantic/Cape_Verde

Africa/Casablanca

Etc/GMT

Europe/London

Atlantic/Reykjavik

Europe/Berlin

Europe/Budapest

Europe/Paris

Europe/Warsaw

Africa/Lagos

Africa/Windhoek

Europe/Bucharest

Asia/Beirut

Africa/Cairo

Asia/Damascus

Африка, Йоханнесбург

Европа, Киев

Европа, Стамбул

Asia/Jerusalem

Asia/Amman

Asia/Baghdad

Europe/Kaliningrad

Asia/Riyadh

Africa/Nairobi

Asia/Tehran

Asia/Dubai

Asia/Baku

Europe/Moscow

Indian/Mauritius

Asia/Tbilisi

Asia/Yerevan

Asia/Kabul

Азия, Карачи

Азия, Ташкент

Азия, Колката

Asia/Colombo

Азия, Катманду

Азия, Астана

Азия, Дакка

Азия, Екатеринбург

Азия, Янгон (Рангун)

Азия, Бангкок

Asia/Novosibirsk

Asia/Shanghai

Asia/Krasnoyarsk

Asia/Singapore

Australia/Perth

Asia/Taipei

Asia/Ulaanbaatar

Asia/Irkutsk

Asia/Tokyo

Asia/Seoul

Australia/Adelaide

Australia/Darwin

Australia/Brisbane

Australia/Sydney

Pacific/Port_Moresby

Australia/Hobart

Asia/Yakutsk

Pacific/Guadalcanal

Asia/Vladivostok

Pacific/Auckland

Etc/GMT-12

Pacific/Fiji

Asia/Magadan

Pacific/Tongatapu

Pacific/Apia

Pacific/Kiritimati

## <a name="json-representation"></a>Описание в формате JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimetimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
