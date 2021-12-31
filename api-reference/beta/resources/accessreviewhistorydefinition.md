---
title: accessReviewHistoryDefinition resource types
description: Представляет коллекцию данных истории обзоров доступа.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8175241c8760986cc821e167e75495cc7f843893
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650617"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>тип ресурса accessReviewHistoryDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет коллекцию данных истории обзоров доступа и области, используемые для сбора этих данных. **ReviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime** **,**  решения и области свойств **accessReviewHistoryDefinition** используются при выборе данных истории отзывов и могут быть изменены. Каждый **объект accessReviewHistoryDefinition** доступен только в течение 30 дней. После того, как состояние определения истории переместилось на ссылку, можно создать для получения данных определения с помощью вызова `done` [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessReviewHistoryDefinitions](../api/accessreviewset-list-historydefinitions.md)|[accessReviewHistoryDefinition collection](accessreviewhistorydefinition.md)|Получите список объектов [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) и их свойств.|
|[Создание accessReviewHistoryDefinition](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создайте новый [объект accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[Получить accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Ознакомьтесь с свойствами и отношениями [объекта accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Создание URI, который можно использовать для получения данных истории отзывов.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[userIdentity](useridentity.md)| Пользователь, создавший это определение истории обзора. |
|createdDateTime|DateTimeOffset|Timestamp, когда было создано определение проверки доступа.|
|решения|Коллекция String|Определяет, какие решения по проверке будут включены в данные истории проверки, если заданы. Необязательный для создания. Все решения будут включены по умолчанию, если не будут предоставлены решения о создании. Возможные значения: `approve` `deny` , , , , `dontKnow` и `notReviewed` `notNotified` .|
|displayName|Строка|Имя для сбора данных истории проверки доступа. Обязательный.|
|downloadUri|Строка|Uri, которые можно использовать для получения данных истории отзывов. Этот URI будет активен в течение 24 часов после сгенерирований.|
|fulfilledDateTime|DateTimeOffset|Timestamp, когда все доступные данные для этого определения были собраны. Это будет установлено после того, как будет заданной для этого определения состояние `done` .|
|id|Строка|Назначен уникальный идентификатор определения истории проверки доступа.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|Timestamp, отзывы, начиная с этой даты или после нее, будут включены в извлеченные данные истории. Обязательный.|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Timestamp, отзывы, начиная с этой даты или до этой даты, будут включены в извлеченные данные истории. Обязательный.|
|scopes|[accessReviewQueryScope](accessreviewqueryscope.md) collection|Используется для области, включаемой отзывов в извлеченные данные истории. Извлекает отзывы, область которых совпадает с этой предоставленной областью. Обязательное.|
|status|Коллекция String|Представляет состояние коллекции данных истории отзывов. Возможные значения: `done`, `inprogress`, `error`, `requested`.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "decisions": [
    {
      "@odata.type": "String"
    }
  ],
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "createdBy": {
    "@odata.type": "#microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    }
  ]
}
```
