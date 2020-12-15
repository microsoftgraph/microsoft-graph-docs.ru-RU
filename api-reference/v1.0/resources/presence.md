---
title: Тип ресурса presence
description: Содержит сведения о присутствии пользователя, включая сведения об их доступности и действиях пользователей.
author: elvinyang-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 1122e14c91a8562757434e4bd36e267ed70790dd
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49675963"
---
# <a name="presence-resource-type"></a>Тип ресурса presence

Пространство имен: microsoft.graph

Содержит сведения о присутствии пользователя, включая сведения об их доступности и действиях пользователей.

> **Примечание.** В настоящее время этот ресурс поддерживается только для пользователей Microsoft Teams.

Этот ресурс поддерживает подписку на уведомления [об изменениях.](/graph/webhooks)

## <a name="methods"></a>Методы

| Метод                                                            | Возвращаемый тип                                       | Описание                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Получить присутствие](../api/presence-get.md)     | [presence](../resources/presence.md)     | Получите сведения о присутствии пользователя.
| [Получить присутствие нескольких пользователей](../api/cloudcommunications-getpresencesbyuserid.md)    |  [коллекция presence](../resources/presence.md)     |  Получите сведения о присутствии для нескольких пользователей.      |


## <a name="properties"></a>Свойства

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  string     |  ИД объекта пользователя   |
|availability    |  string collection   |   Базовые сведения о присутствии для пользователя. Возможные значения: `Available` , , , , `AvailableIdle`  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`  |
|activity    |  string collection      |    Дополнительная информация о доступности пользователя. Возможные значения: `Available` , , , , , , `Away` , `BeRightBack` , `Busy` , `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .       |

>**Примечание.** Дополнительные данные о различных состояниях присутствия см. в [записях о присутствии пользователей в Teams.](/microsoftteams/presence-admins) 

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.presence"
}-->
```json
{
   "id":"string",
   "availability":"string",
   "activity":"string"
}
```
