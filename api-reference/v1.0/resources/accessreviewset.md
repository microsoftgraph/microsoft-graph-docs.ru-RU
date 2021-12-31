---
title: тип ресурсов accessReviewSet
description: Контейнер для базовых ресурсов, которые раскрывают API обзоров доступа и функций. В настоящее время предоставляется только ресурс accessReviewScheduleDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f1d3b28da541a365d1507cefce8d18adbc407dae
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650839"
---
# <a name="accessreviewset-resource-type"></a>тип ресурсов accessReviewSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для базовых ресурсов, которые раскрывают API обзоров доступа и функций. В настоящее время предоставляется [только связь accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)

Наследует от [объекта](entity.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|определения|[accessReviewScheduleDefinition collection](../resources/accessreviewscheduledefinition.md)| Представляет шаблон и планирование просмотра доступа. |

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

