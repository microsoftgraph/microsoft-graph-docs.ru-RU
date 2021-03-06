---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: d6f88f23a6c08d5aa757163d4956c104a603e87b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515634"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.

> **Примечание:** В настоящее время этот ресурс поддерживается только для пользователей Microsoft Teams.

Этот ресурс поддерживает подписку на изменение [уведомлений.](/graph/webhooks)

## <a name="methods"></a>Методы

| Метод                                                            | Возвращаемый тип                                       | Описание                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Получить присутствие](../api/presence-get.md)     | [presence](../resources/presence.md)     | Получите сведения о присутствии пользователя.
| [Наличие нескольких пользователей](../api/cloudcommunications-getpresencesbyuserid.md)    |  [Коллекция присутствия](../resources/presence.md)     |  Получите сведения о присутствии для нескольких пользователей.      |


## <a name="properties"></a>Свойства

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  string     |  ID объекта пользователя   |
|availability    |  string collection   |   Базовые сведения о присутствии пользователя. Возможные значения `Available` : , , , , `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` , `Offline``PresenceUnknown`  |
|действие    |  string collection      |    Дополнительные сведения о доступности пользователя. Возможные `Available` значения: , , , , , , , , `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .       |
|outOfOfficeSettings | [outOfOfficeSettings](outOfOfficeSettings.md) | Параметры вне офиса для пользователя. |

>**Примечание:** Дополнительные данные о различных состояниях присутствия см. в [записи Присутствия пользователя в Teams.](/microsoftteams/presence-admins) 

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
