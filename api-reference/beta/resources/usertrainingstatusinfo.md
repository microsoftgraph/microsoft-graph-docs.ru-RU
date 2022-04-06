---
title: тип ресурса userTrainingStatusInfo
description: Представляет назначенное обучение и его состояние для пользователя в имитации атаки и обучении.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: d9e2900bb2c72ba8100d5fe49130b7229db988ee
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757845"
---
# <a name="usertrainingstatusinfo-resource-type"></a>тип ресурса userTrainingStatusInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначенное обучение и его состояние для пользователя в имитации атаки и обучении.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedDateTime|DateTimeOffset|Дата и время назначения обучения пользователю.|
|completionDateTime|DateTimeOffset|Дата и время завершения обучения пользователем.|
|displayName|String|Отображение имени назначенного обучения.|
|trainingStatus|trainingStatus|Состояние обучения, назначенного пользователю. Возможные значения: `unknown`, `assigned`, `inProgress`, `completed`, `overdue`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingStatusInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingStatusInfo",
  "assignedDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "trainingStatus": "String",
  "displayName": "String"
}
```

