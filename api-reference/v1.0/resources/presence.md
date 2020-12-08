---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.
author: elvinyang-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 52c726ab1e5b9d50a81797bc2d2375bee3793a2a
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581268"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Пространство имен: microsoft.graph

Содержит сведения о присутствии пользователя, в том числе сведения о доступности и активности пользователей.

> **Примечание:** Этот ресурс в настоящее время поддерживается только для пользователей Microsoft Teams.

Этот ресурс поддерживает подписку на [уведомления об изменениях](/graph/webhooks).

## <a name="methods"></a>Методы

| Метод                                                            | Возвращаемый тип                                       | Описание                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Получение сведений о присутствии](../api/presence-get.md)     | [presence](../resources/presence.md)     | Получение сведений о присутствии пользователя.
| [Получение сведений о присутствии нескольких пользователей](../api/cloudcommunications-getpresencesbyuserid.md)    |  Коллекция [присутствия](../resources/presence.md)     |  Получение сведений о присутствии для нескольких пользователей.      |


## <a name="properties"></a>Свойства

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|id    |  string     |  Идентификатор объекта пользователя   |
|availability    |  string collection   |   Базовые сведения о присутствии для пользователя. Возможные значения:,,,,,,, `Available` `AvailableIdle`  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`  |
|activity    |  string collection      |    Дополнительная информация о доступности пользователя. Возможные значения:,,,,,,,,,,, `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` , `Presenting` , `UrgentInterruptionsOnly` .       |

>**Примечание:** Чтобы узнать больше о различных состояниях присутствия, ознакомьтесь с разделом сведения о [присутствии пользователей в Teams](/microsoftteams/presence-admins). 

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