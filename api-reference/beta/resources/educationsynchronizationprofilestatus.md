---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e3cc519f30b571d6c69dce48b74cd70da7f58e6f
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792816"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>Тип ресурса Едукатионсинчронизатионпрофилестатус

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
