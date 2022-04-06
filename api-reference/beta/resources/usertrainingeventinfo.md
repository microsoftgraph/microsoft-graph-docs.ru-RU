---
title: тип ресурса userTrainingEventInfo
description: Представляет события обучения, назначенного пользователю в кампании моделирования атак и обучения.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1a33cba93e61752d33b9829871b3280955895360
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758293"
---
# <a name="usertrainingeventinfo-resource-type"></a>тип ресурса userTrainingEventInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет события обучения, назначенного пользователю в кампании моделирования атак и обучения. Учебные мероприятия включают назначение обучения, обновление обучающих работ и завершение обучения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображение имени тренинга.|
|latestTrainingStatus|trainingStatus|Последний статус обучения, назначенного пользователю. Возможные значения: `unknown`, `assigned`, `inProgress`, `completed`, `overdue`, `unknownFutureValue`.|
|trainingAssignedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|Сведения о событии обучения при его присвоении пользователю.|
|trainingCompletedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|Сведения о событиях обучения, когда оно было завершено пользователем.|
|trainingUpdatedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|Сведения о событии обучения, когда оно было обновлено или в процессе выполнения пользователем.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingEventInfo",
  "displayName": "String",
  "latestTrainingStatus": "String",
  "trainingAssignedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  },
  "trainingUpdatedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  },
  "trainingCompletedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  }
}
```

