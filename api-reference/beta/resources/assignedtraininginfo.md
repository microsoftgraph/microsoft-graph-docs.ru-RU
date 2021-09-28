---
title: тип ресурса assignedTrainingInfo
description: Представляет сведения о назначенном обучении в кампании моделирования атак и обучения.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 15caed31f7db60980e453e942653820dc8b348bc
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979792"
---
# <a name="assignedtraininginfo-resource-type"></a>тип ресурса assignedTrainingInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о назначении обучения в кампании моделирования атак и обучения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedUserCount|Int32|Количество пользователей, которым назначено обучение в кампании моделирования и обучения атак.|
|completedUserCount|Int32|Число пользователей, завершивших обучение в кампании моделирования атак и обучения.|
|displayName|Строка|Отображение имени тренинга в кампании моделирования атак и учебной кампании.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignedTrainingInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignedTrainingInfo",
  "assignedUserCount": "Integer",
  "completedUserCount": "Integer",
  "displayName": "String"
}
```

