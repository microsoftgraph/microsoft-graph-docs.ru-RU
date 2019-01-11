---
title: Тип ресурса dateTimeTimeZone
description: Описывает дату, время и часовой пояс для определенного момента.
localization_priority: Priority
ms.openlocfilehash: 9bec62c21f97c58b915ecc40010f8030ea760825
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827330"
---
# <a name="datetimetimezone-resource-type"></a>Тип ресурса dateTimeTimeZone

Описывает дату, время и часовой пояс для определенного момента.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|dateTime|String|Один момент времени в объединенном представлении даты и времени (`<date>T<time>`).|
|timeZone|String|Один из указанных ниже часовых поясов.|

Свойство _TimeZone_ можно задать для каждого из часовых поясов, которые поддерживаются в Windows, а также для указанных ниже часовых поясов.

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

Ниже представлено описание ресурса в формате JSON.

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
<!-- {
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
