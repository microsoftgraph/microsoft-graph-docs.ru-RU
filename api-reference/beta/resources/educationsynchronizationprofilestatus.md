---
title: тип ресурса educationSynchronizationProfileStatus
description: 'Представляет состояние синхронизации профиля синхронизации школьных данных. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 55636a78cd904c6992de0cf48ab333ccef8bb84a
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534195"
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
| id                          | Строка                         | Уникальный идентификатор ресурса. (только для чтения)                                                                      |
| status                      | educationSynchronizationStatus | Состояние синхронизации. Возможные значения: `paused` `inProgress` , , , , , `success` `error` `quarantined` `validationError` , `extracting` *`validating`*. |
| lastSynchronizationDateTime | DateTimeOffset                 | Представляет время последней успешной синхронизации.                                        |
| lastActivityDateTime | DateTimeOffset                 | Представляет время, когда последние изменения наблюдались в профиле.                                        |
| errorCount | Целое                 | Количество ошибок при синхронизации.                                        |
| statusMessage | Строка                 | Сообщение о состоянии для текущего этапа синхронизации профиля.                                        |

Статусы "Извлечение" и "Проверка" возвращаются только для приложений, подготовленных для обработки новых участников. Выбор в этом вопросе делается путем установки заглавного загона http prefer request: `Prefer: include-unknown-enum-members` . Дополнительные новости: [эволюционируемые enums](/graph/best-practices-concept#evolvable-enums).


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
