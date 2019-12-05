---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 15635f29143a51f87a107c5f4e632b8684e79c50
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844283"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.

> **Примечание:** Этот ресурс в настоящее время поддерживается только для пользователей Microsoft Teams.

## <a name="methods"></a>Методы

| Метод                                                            | Возвращаемый тип                                       | Описание                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Получение сведений о присутствии](../api/presence-get.md)     | [знак](../resources/presence.md)     | Получение сведений о присутствии пользователя.
| [Получение сведений о присутствии нескольких пользователей](../api/cloudcommunications-getpresencesbyuserid.md)    |  Коллекция [присутствия](../resources/presence.md)     |  Получение сведений о присутствии для нескольких пользователей.      |


## <a name="properties"></a>Свойства

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  string     |  Идентификатор объекта пользователя   |
|availability    |  string collection   |   Базовые сведения о присутствии для пользователя. Возможные значения: `Available`, `AvailableIdle`, `Away`, `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb`,,,, `Offline`,`PresenceUnknown`  |
|activity    |  string collection      |    Дополнительная информация о доступности пользователя. Возможные значения: `Available`, `Away`, `BeRightBack`,`Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `PresenceUnknown``Presenting` `UrgentInterruptionsOnly`,,,,,,,,,,. `Inactive``InAMeeting` `Offline` `OffWork``OutOfOffice`       |

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
