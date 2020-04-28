---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 797ddac8bc582cd5e5d4d51e0e1ad94645c3c1e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521574"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Пространство имен: microsoft.graph

Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.

> **Примечание:** Этот ресурс в настоящее время поддерживается только для пользователей Microsoft Teams.

## <a name="methods"></a>Методы

| Метод                                                            | Возвращаемый тип                                       | Описание                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Получение сведений о присутствии](../api/presence-get.md)     | [presence](../resources/presence.md)     | Получение сведений о присутствии пользователя.
| [Получение сведений о присутствии нескольких пользователей](../api/cloudcommunications-getpresencesbyuserid.md)    |  Коллекция [присутствия](../resources/presence.md)     |  Получение сведений о присутствии для нескольких пользователей.      |


## <a name="properties"></a>Свойства

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  string     |  Идентификатор объекта пользователя   |
|availability    |  Коллекция строк   |   Базовые сведения о присутствии для пользователя. Возможные значения: `Available`, `AvailableIdle`, `Away`, `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb`,,,, `Offline`,`PresenceUnknown`  |
|activity    |  Коллекция строк      |    Дополнительная информация о доступности пользователя. Возможные значения: `Available`, `Away`, `BeRightBack`,`Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `PresenceUnknown``Presenting` `UrgentInterruptionsOnly`,,,,,,,,,,. `Inactive``InAMeeting` `Offline` `OffWork``OutOfOffice`       |

>**Примечание:** Чтобы узнать больше о различных состояниях присутствия, ознакомьтесь с разделом сведения о [присутствии пользователей в Teams](https://docs.microsoft.com/microsoftteams/presence-admins). 

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
