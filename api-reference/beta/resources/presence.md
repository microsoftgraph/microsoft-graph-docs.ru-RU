---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 4743cef5b2772f636d7c40118a11e886839acc95
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334018"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.

> **Примечание:** В настоящее время этот ресурс поддерживается только для Microsoft Teams пользователей.

Этот ресурс поддерживает подписку на изменение [уведомлений](/graph/webhooks).

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

| Свойство        | Тип                                          | Описание                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                  | string                                        | ID объекта пользователя                                                                                                                                                                                                                                                                             |
| availability        | string collection                             | Базовые сведения о присутствии пользователя. Возможные значения : `Available`, , , , `Busy`, `DoNotDisturb``BusyIdle``Offline``BeRightBack``Away``AvailableIdle``PresenceUnknown`                                                                                                           |
| действие            | string collection                             | Дополнительные сведения о доступности пользователя. Возможные значения: `Available`, `Away``BeRightBack`, , `Busy`, `DoNotDisturb`, `InACall`, , `Inactive``InAConferenceCall``InAMeeting``PresenceUnknown``Offline``UrgentInterruptionsOnly``OffWork``OutOfOffice``Presenting`. |
| outOfOfficeSettings | [outOfOfficeSettings](outOfOfficeSettings.md) | Параметры вне офиса для пользователя.                                                                                                                                                                                                                                                         |

>**Примечание:** Дополнительные данные о различных состояниях присутствия см. [в Teams.](/microsoftteams/presence-admins) 

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
