---
title: Тип ресурса educationSynchronizationProfileStatus
description: 'Представляет состояние синхронизации профилей синхронизации данных school. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1fd77f48544e5e6bc0c582e4ce9fb2a5b1b6601a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396156"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>Тип ресурса educationSynchronizationProfileStatus

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет состояния синхронизации данных school [синхронизации профилей](educationsynchronizationprofile.md). 

> **Примечание:** Обновления для **educationSynchronizationProfileStatus** может отложить из-за асинхронной фоновой синхронизации обработки.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | Возвращает состояние определенного синхронизации профилей. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **status** | educationSynchronizationStatus | Состояние синхронизации. Возможные значения: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`. |
| **lastSynchronizationDateTime** | DateTimeOffset | Представляет время, когда наблюдались последних изменений в каталоге.  |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
