---
title: тип ресурса attackSimulationRepeatOffender
description: Представляет пользователя-рецидививчика в имитации атаки и обучении.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: a78d474514a4975584425c18da71451dc0352e25
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979707"
---
# <a name="attacksimulationrepeatoffender-resource-type"></a>тип ресурса attackSimulationRepeatOffender

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователя в клиенте, который не раз удавлялся атакам в различных кампаниях по моделированию атак и обучению.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|Пользователь в кампании моделирования атак и обучения.|
|repeatOffenceCount|Int32|Количество повторных правонарушений пользователя в имитации атак и учебных кампаниях.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationRepeatOffender"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationRepeatOffender",
  "repeatOffenceCount": "Integer",
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

