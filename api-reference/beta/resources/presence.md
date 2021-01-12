---
title: Тип ресурса presence
description: Содержит сведения о присутствии пользователя, включая сведения об их доступности и действиях пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: ddbe555df37d232940bb8eadb081be459d0f8562
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796579"
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
|availability    |  Коллекция строк   |   Базовые сведения о присутствии для пользователя. Возможные значения: `Available` `AvailableIdle` , , `Away` `BeRightBack` , `Busy` `BusyIdle` `DoNotDisturb` `Offline``PresenceUnknown`  |
|действие    |  Коллекция строк      |    Дополнительная информация о доступности пользователя. Возможные значения: `Available` `Away` , `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .       |
|outOfOfficeSettings | [outOfOfficeSettings](outOfOfficeSettings.md) | Параметры "Нет на месте" для пользователя. |

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
   "activity":"string",
   "outOfOfficeSettings":{"@odata.type": "#microsoft.graph.outOfOfficeSettings"}
}
```
