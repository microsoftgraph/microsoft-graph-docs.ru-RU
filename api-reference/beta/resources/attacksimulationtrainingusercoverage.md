---
title: тип ресурса attackSimulationTrainingUserCoverage
description: Представляет обучающий охват для пользователя в имитации атак и обучении.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: ac8772817fa4c5887a1ae84c80165794b4bed16c
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979776"
---
# <a name="attacksimulationtrainingusercoverage-resource-type"></a>тип ресурса attackSimulationTrainingUserCoverage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет накопительные обучающие данные для пользователя в имитации атаки и обучении.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|Пользователь в кампании моделирования атак и обучения.|
|userTrainings|[коллекция userTrainingStatusInfo](../resources/usertrainingstatusinfo.md)|Список назначенных тренингов и их состояния для пользователя.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationTrainingUserCoverage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationTrainingUserCoverage",
  "userTrainings": [
    {
      "@odata.type": "microsoft.graph.userTrainingStatusInfo"
    }
  ],
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

