---
title: тип ресурсов accessReviewSet
description: Контейнер для базовых ресурсов, которые раскрывают API обзоров доступа и функций. В настоящее время предоставляется только ресурс accessReviewScheduleDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4964b26b1f6c415a0e822c6d47e67499876011b1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333220"
---
# <a name="accessreviewset-resource-type"></a>тип ресурсов accessReviewSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для базовых ресурсов, которые раскрывают API обзоров доступа и функций. В настоящее время предоставляется [только связь accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

Наследуется [от сущности](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|определения|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)| Представляет шаблон и планирование просмотра доступа. |
|historyDefinitions|[accessReviewHistoryDefinition collection](../resources/accessreviewhistorydefinition.md)| Представляет коллекцию данных истории обзоров доступа и области, используемые для сбора этих данных.|

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

