---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: jsandoval-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 6de4f4f63302bfa8e1229f60c6aad77b1abe1fd8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962429"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Пространство имен: microsoft.graph

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
|availability    |  Коллекция строк   |   Базовые сведения о присутствии пользователя. Возможные значения `Available` : , , , , `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` , `Offline``PresenceUnknown`  |
|действие    |  Коллекция строк      |    Дополнительные сведения о доступности пользователя. Возможные `Available` значения: , , , , , , , , `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .       |

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
   "activity":"string"
}
```
