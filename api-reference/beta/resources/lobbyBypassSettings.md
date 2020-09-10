---
title: Тип ресурса Лоббибипасссеттингс
description: Указывает, какие участники могут обходить зал собрания.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3723f6593547b75c60a82b8436995c931d64e436
ms.sourcegitcommit: 7dcae492d8b4707d068adca3a74732e25a8198e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2020
ms.locfileid: "47423688"
---
# <a name="lobbybypasssettings-resource-type"></a>Тип ресурса Лоббибипасссеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, какие участники могут обходить зал собрания.

## <a name="properties"></a>Свойства

| Свойство              | Тип    | Описание                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| scope                 | лоббибипассскопе  | Указывает тип участников, которые автоматически отправляются на собрание, минуя "зал ожидания". Возможные значения перечислены в следующей таблице. Необязательный параметр.|
| исдиалинбипассенаблед | Boolean | Указывает, следует ли всегда разрешать абонентам с телефонным подключением обходить "зал ожидания". Необязательный параметр. | 

### <a name="lobbybypassscope-values"></a>значения Лоббибипассскопе

| Значение                    | Описание                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| organizer                | Только организатор дойдет на собрание, минуя "зал ожидания". Все остальные участники помещаются в зал собрания.                                                                                                         |
| organization;             | Только участники одной компании могут присутствовать на собрании, минуя "зал ожидания". Все остальные участники помещаются в зал собрания.                                                                              |
| организатионандфедератед | Только участники одной компании или доверенной Организации доходят на собрание, минуя "зал ожидания". Все остальные участники помещаются в зал собрания. |
| просматривающи                 | Все пользователи размещаются на собрании. В зал собрания не помещаются участники.                                                                                                                   |
| unknownFutureValue       | Неизвестное будущее значение.                                                                                                                                     |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "organizer | organization | organizationAndFederated | everyone | unknownFutureValue",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
