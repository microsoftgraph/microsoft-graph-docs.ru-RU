---
title: тип ресурса accessReviewHistoryInstance
description: Представляет собой повторение объекта accessReviewHistoryDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f2e3c73dc7b5f368db20ab6b84f58b637099cb7b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337694"
---
# <a name="accessreviewhistoryinstance-resource-type"></a>тип ресурса accessReviewHistoryInstance

Пространство имен: microsoft.graph

 Представляет собой повторение объекта [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) . Определение истории, которое не повторяется, будет иметь точно один экземпляр.

 Каждый **accessReviewHistoryInstance** вместе со связанным с ним **accessReviewHistoryDefinition** содержит обзор **свойствHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime****, решения**, **scheduleSettings** и **области**. Эти свойства используются при планировании повторений, а также при выборе данных обзора и могут быть изменены. **Каждый объект и данные accessReviewHistoryInstance** доступны только в течение 30 дней. После того, как состояние **accessReviewHistoryInstance** `done` было перемещено на ссылку, можно создать для получения данных экземпляра с помощью вызова [generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md).

## <a name="methods"></a>Методы

| Метод  | Тип возвращаемых данных | Описание |
|:---|:---|:---|
|[Список accessReviewHistoryInstances](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md) collection| Извлечение списка [объектов accessReviewHistoryInstance](accessreviewhistoryinstance.md) и их свойств.|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создает URI, который можно использовать для получения данных истории отзывов экземпляра.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|downloadUri|Строка|Uri, которые можно использовать для получения данных истории отзывов. Этот URI будет активен в течение 24 часов после сгенерирований. Обязательный элемент.|
|expirationDateTime|DateTimeOffset|Timestamp, когда истекает срок действия этого экземпляра и связанных данных, а история удаляется. Обязательный элемент.|
|fulfilledDateTime|DateTimeOffset|Timestamp, когда все доступные данные для этого экземпляра были собраны. Это будет установлено после того, как будет заданной для этого экземпляра состояние `done`. Обязательный.|
|id|Строка|Назначен уникальный идентификатор экземпляра истории проверки доступа. Только для чтения. Обязательный.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|Timestamp, отзывы, заканчивающийся до этой даты, будут включены в извлеченные данные истории.|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Timestamp, отзывы, начиная с этой даты или после нее, будут включены в извлеченные данные истории.|
|runDateTime|DateTimeOffset|Timestamp, когда планируется сгенерирование данных истории экземпляра.|
|status|accessReviewHistoryStatus|Представляет состояние коллекции данных истории отзывов. Допустимые значения: `done`, `inProgress`, `error`, `requested`, `unknownFutureValue`. После того **как состояние** было отмечено как `done`, для получения данных экземпляра можно создать ссылку, вызывав [метод generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md) .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryInstance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryInstance",
  "id": "String (identifier)",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "status": "String",
  "runDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "expirationDateTime": "String (timestamp)"
}
```
