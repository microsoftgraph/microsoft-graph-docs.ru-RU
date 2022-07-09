---
title: Тип ресурса accessReviewSet
description: Контейнер для базовых ресурсов, предоставляющих API и функции проверок доступа. В настоящее время предоставляется только ресурс accessReviewScheduleDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a4310978c8c3578604523f9fa299581f5b24039a
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697976"
---
# <a name="accessreviewset-resource-type"></a>Тип ресурса accessReviewSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для базовых ресурсов, предоставляющих API и функции проверок доступа. В настоящее время предоставляется только [связь accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

Наследует [от сущности](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|Определения|[Коллекция accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)| Представляет шаблон и планирование проверки доступа. |
|historyDefinitions|[Коллекция accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md)| Представляет коллекцию данных журнала проверки доступа и областей, используемых для сбора этих данных.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewSet"
}
```

