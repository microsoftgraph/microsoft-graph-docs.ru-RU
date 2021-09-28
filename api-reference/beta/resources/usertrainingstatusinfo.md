---
title: тип ресурса userTrainingStatusInfo
description: Представляет назначенное обучение и его состояние для пользователя в имитации атаки и обучении.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 82b0c6b1de49c9b8eb0572dab33fca8c90e2b6fe
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979756"
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
|displayName|Строка|Отображение имени назначенного обучения.|
|trainingStatus|trainingStatus|Состояние обучения, назначенного пользователю. Возможные значения: `unknown`, `assigned`, `inProgress`, `completed`, `overdue`, `notCompleted`, `unknownFutureValue`.|

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

