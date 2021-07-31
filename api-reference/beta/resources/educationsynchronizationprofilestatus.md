---
title: тип ресурса educationSynchronizationProfileStatus
description: 'Представляет состояние синхронизации профиля синхронизации школьных данных. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ee802e9749418b9a1d2a9bbdbe3916493e5cf431
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665909"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>тип ресурса educationSynchronizationProfileStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние синхронизации профиля синхронизации школьных [данных.](educationsynchronizationprofile.md)

> **Примечание:** Обновления в **educationSynchronizationProfileStatus** могут быть отложены из-за асинхронного характера обработки фоновой синхронизации.

## <a name="methods"></a>Методы

| Метод                                                                      | Возвращаемый тип                               | Описание                                              |
| :-------------------------------------------------------------------------- | :---------------------------------------- | :------------------------------------------------------- |
| [Получить состояние синхронизации](../api/educationsynchronizationprofilestatus-get.md) | **educationSynchronizationProfileStatus** | Возвращаем состояние определенного профиля синхронизации. |

## <a name="properties"></a>Свойства

| Свойство                    | Тип                           | Описание                                                                                                              |
| :-------------------------- | :----------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| id                          | String                         | Уникальный идентификатор ресурса. (только для чтения)                                                                      |
| status                      | educationSynchronizationStatus | Состояние синхронизации. Возможные значения: `paused` `inProgress` , , , , , , `success` `error` `validationError` `quarantined` `unknownFutureValue` `extracting` `validating` . Обратите внимание, что для получения следующих значений в этом развиваемом переуме- `Prefer: include-unknown-enum-members` [](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `extracting` `validating`|
| lastSynchronizationDateTime | DateTimeOffset                 | Представляет время последней успешной синхронизации.                                        |
| lastActivityDateTime | DateTimeOffset                 | Представляет время, когда последние изменения наблюдались в профиле.                                        |
| errorCount | Целое                 | Количество ошибок при синхронизации.                                        |
| statusMessage | String                 | Сообщение о состоянии для текущего этапа синхронизации профиля.                                        |


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
  "id": "String",
  "status": { "@odata.type": "microsoft.graph.educationSynchronizationStatus" },
  "lastSynchronizationDateTime": "DateTimeOffset",
  "lastActivityDateTime": "DateTimeOffset",
  "errorCount": "Int",
  "statusMessage": "String"
}
```
