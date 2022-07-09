---
title: Тип ресурса accessReviewHistoryInstance
description: Представляет повторение объекта accessReviewHistoryDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c6b1d137c470bdf384bc60d2a20834860f7dbd01
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697913"
---
# <a name="accessreviewhistoryinstance-resource-type"></a>Тип ресурса accessReviewHistoryInstance

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 Представляет повторение объекта [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) . Определение журнала, которое не является повторяемой, будет иметь ровно один экземпляр.

 Каждый **объект accessReviewHistoryInstance** вместе со связанным **accessReviewHistoryDefinition** содержит свойства **reviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime****, решения**, **scheduleSettings** и **области**. Эти свойства используются при планировании повторений, а также при выборе данных проверки и могут быть изменены. **Каждый объект и данные accessReviewHistoryInstance** доступны только в течение 30 дней. После перемещения **состояния accessReviewHistoryInstance** `done` в ссылку можно создать для получения данных экземпляра путем вызова [generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md).

## <a name="methods"></a>Методы

| Метод  | Тип возвращаемых данных | Описание |
|:---|:---|:---|
|[Перечисление объектов accessReviewHistoryInstance](../api/accessreviewhistorydefinition-list-instances.md)|[Коллекция accessReviewHistoryInstance](accessreviewhistoryinstance.md)| Получение списка объектов [accessReviewHistoryInstance](accessreviewhistoryinstance.md) и их свойств.|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создает универсальный код ресурса (URI), который можно использовать для получения данных журнала проверки экземпляра.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|downloadUri|Строка|Универсальный код ресурса (URI), который можно использовать для получения данных журнала проверки. Этот URI будет активен в течение 24 часов после создания. Обязательный элемент.|
|expirationDateTime|DateTimeOffset|Метка времени, когда истекает срок действия этого экземпляра и связанных данных, а журнал удаляется. Обязательный элемент.|
|fulfilledDateTime|DateTimeOffset|Метка времени сбора всех доступных данных для этого экземпляра. Он будет установлен после того, как для этого экземпляра будет установлено состояние `done`. Обязательный.|
|id|Строка|Назначенный уникальный идентификатор экземпляра журнала проверки доступа. Только для чтения. Обязательный.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|Метка времени, проверки, заканчивающиеся на эту дату или до этой даты, будут включены в извлеченные данные журнала.|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Метка времени, проверки, начиная с этой даты или после нее, будут включены в извлеченные данные журнала.|
|runDateTime|DateTimeOffset|Метка времени, когда планируется создание данных журнала экземпляра.|
|status|accessReviewHistoryStatus|Представляет состояние сбора данных журнала проверки. Допустимые значения: `done`, `inProgress`, `error`, `requested`, `unknownFutureValue`. После **пометки** состояния `done`можно создать ссылку для получения данных экземпляра путем вызова [метода generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md) .|

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
