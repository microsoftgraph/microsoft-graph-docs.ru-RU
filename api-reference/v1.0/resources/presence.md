---
title: Тип ресурса присутствия
description: Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 4343c79e9c81b83f91fb341131a8ef9ad8b2f607
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333864"
---
# <a name="presence-resource-type"></a>Тип ресурса присутствия

Пространство имен: microsoft.graph

Содержит сведения о присутствии пользователя, включая его доступность и активность пользователей.

> **Примечание:** В настоящее время этот ресурс поддерживается только для Microsoft Teams пользователей.

Этот ресурс поддерживает подписку на изменение [уведомлений](/graph/webhooks).

## <a name="methods"></a>Методы

| Метод                                                                               | Возвращаемый тип                                     | Описание                                         |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :-------------------------------------------------- |
| [Получить присутствие](../api/presence-get.md)                                               | [presence](../resources/presence.md)            | Получите сведения о присутствии пользователя.                  |
| [Наличие нескольких пользователей](../api/cloudcommunications-getpresencesbyuserid.md) | [Коллекция присутствия](../resources/presence.md) | Получите сведения о присутствии для нескольких пользователей.    |
| [Настройка присутствия](../api/presence-setpresence.md)                                       |                                                 | Установите сеанс присутствия приложения для пользователя.   |
| [Четкое присутствие](../api/presence-clearpresence.md)                                   |                                                 | Очистить сеанс присутствия приложения для пользователя. |

## <a name="properties"></a>Свойства

| Свойство | Тип              | Описание                                                                                                                                                                                                                                                                                       |
| :----------- | :---------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| id           | string            | ID объекта пользователя                                                                                                                                                                                                                                                                                |
| availability | string collection | Базовые сведения о присутствии пользователя. Возможные значения : `Available`, , , , `Busy`, `DoNotDisturb``BusyIdle``Offline``BeRightBack``Away``AvailableIdle``PresenceUnknown`                                                                                                              |
| действие     | string collection | Дополнительные сведения о доступности пользователя. Возможные значения: `Available`, , , , `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive``OffWork``Presenting``OutOfOffice``UrgentInterruptionsOnly``PresenceUnknown``Offline``InAMeeting`, . `Busy``BeRightBack``Away` |

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
   "activity":"string"
}
```
