---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 257167fe5b7d417751771650f8e5f03b3dd66296
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107692"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.

> **Примечание:** В настоящее время этот ресурс поддерживается только для Microsoft Teams пользователей.

Этот ресурс поддерживает подписку на изменение [уведомлений.](/graph/webhooks)

## <a name="methods"></a>Методы

| Метод                                                                               | Возвращаемый тип                                     | Описание                                      |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :----------------------------------------------- |
| [Получить присутствие](../api/presence-get.md)                                               | [presence](../resources/presence.md)            | Получите сведения о присутствии пользователя.               |
| [Наличие нескольких пользователей](../api/cloudcommunications-getpresencesbyuserid.md) | [Коллекция присутствия](../resources/presence.md) | Получите сведения о присутствии для нескольких пользователей. |
| [Настройка присутствия](../api/presence-setpresence.md)                                               |                                                 | Установите сеанс присутствия приложения для пользователя.           |
| [Четкое присутствие](../api/presence-clearpresence.md)                                           |                                                 | Очистить сеанс присутствия приложения для пользователя.         |

## <a name="properties"></a>Свойства

| Связь        | Тип                                          | Описание                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                  | string                                        | ID объекта пользователя                                                                                                                                                                                                                                                                             |
| availability        | Коллекция строк                             | Базовые сведения о присутствии пользователя. Возможные значения `Available` : , , , , `AvailableIdle` `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` , `Offline``PresenceUnknown`                                                                                                           |
| действие            | Коллекция строк                             | Дополнительные сведения о доступности пользователя. Возможные `Available` значения: , , , , , , , , `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` . |
| outOfOfficeSettings | [outOfOfficeSettings](outOfOfficeSettings.md) | Параметры вне офиса для пользователя.                                                                                                                                                                                                                                                         |

>**Примечание:** Дополнительные данные о различных состояниях присутствия см. в [Teams.](/microsoftteams/presence-admins) 

## <a name="relationships"></a>Отношения

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
