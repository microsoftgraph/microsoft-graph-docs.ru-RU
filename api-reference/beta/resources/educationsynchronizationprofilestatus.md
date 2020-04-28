---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88e2f85cc4b24bd55cdfc1fbc5aeecd7bee8c461
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500032"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>Тип ресурса Едукатионсинчронизатионпрофилестатус

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md). 

> **Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md) | **едукатионсинчронизатионпрофилестатус** | Возврат состояния определенного профиля синхронизации. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **status** | едукатионсинчронизатионстатус | Состояние синхронизации. Возможные `paused`значения:, `inProgress`, `success`, `error`, `quarantined`,. `validationError` |
| **ластсинчронизатиондатетиме** | DateTimeOffset | Представляет время, в течение которого последние изменения были просмотрены в каталоге.  |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
