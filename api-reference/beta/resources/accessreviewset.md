---
title: Тип ресурса accessReviewSet
description: Контейнер для базовых ресурсов, предоставляющих API и функции проверок доступа. В настоящее время предоставляется только ресурс accessReviewScheduleDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ca33119169ed61604b0c9deed18ecad33bd76069
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697850"
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
|Решения|[Коллекция accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)| Представляет Azure AD проверки доступа для экземпляра проверки.|
|Определения|[Коллекция accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)| Представляет шаблон и планирование проверки доступа. |
|historyDefinitions|[Коллекция accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md)| Представляет коллекцию данных журнала проверки доступа и областей, используемых для сбора этих данных.|
|policy|[accessReviewPolicy](../resources/accessreviewpolicy.md)| Ресурс, позволяющий администраторам управлять политиками проверки доступа на уровне каталога в своем клиенте.|

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

