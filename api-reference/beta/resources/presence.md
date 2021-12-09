---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 8589be83cc647952676b7f0059c60c1d60778b91
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390992"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.

> **Примечание:** В настоящее время этот ресурс поддерживается только для Microsoft Teams пользователей.

Этот ресурс поддерживает подписку на изменение [уведомлений.](/graph/webhooks)

## <a name="methods"></a>Методы

| Метод                                                                               | Возвращаемый тип                                     | Описание                                                                       |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :-------------------------------------------------------------------------------- |
| [Получить присутствие](../api/presence-get.md)                                               | [presence](../resources/presence.md)            | Получите сведения о присутствии пользователя.                                                |
| [Наличие нескольких пользователей](../api/cloudcommunications-getpresencesbyuserid.md) | [Коллекция присутствия](../resources/presence.md) | Получите сведения о присутствии для нескольких пользователей.                                  |
| [Настройка присутствия](../api/presence-setpresence.md)                                       |                                                 | Установите состояние доступности и активности [в](../api/presence-setpresence.md#presence-sessions) сеансе присутствия приложения для пользователя. |
| [Четкое присутствие](../api/presence-clearpresence.md)                                   |                                                 | Очистить сеанс присутствия приложения для пользователя.                                       |
| [Настройка предпочтительного присутствия пользователя](../api/presence-setuserpreferredpresence.md)           |                                                 | Установите предпочтительное состояние доступности и активности для пользователя.                    |
| [Четкое предпочтительное присутствие пользователя](../api/presence-clearuserpreferredpresence.md)       |                                                 | Очистка предпочтительного состояния доступности и активности для пользователя.                  |

## <a name="properties"></a>Свойства

| Связь        | Тип                                          | Описание                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                  | string                                        | ID объекта пользователя                                                                                                                                                                                                                                                                             |
| availability        | string collection                             | Базовые сведения о присутствии пользователя. Возможные значения `Available` : , , , , `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` , `Offline``PresenceUnknown`                                                                                                           |
| действие            | string collection                             | Дополнительные сведения о доступности пользователя. Возможные `Available` значения: , , , , , , , , `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` . |
| outOfOfficeSettings | [outOfOfficeSettings](outOfOfficeSettings.md) | Параметры вне офиса для пользователя.                                                                                                                                                                                                                                                         |

>**Примечание:** Дополнительные данные о различных состояниях присутствия см. в [Teams.](/microsoftteams/presence-admins) 

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
