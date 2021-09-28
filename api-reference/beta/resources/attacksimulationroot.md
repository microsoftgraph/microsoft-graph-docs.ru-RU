---
title: тип ресурса attackSimulationRoot
description: Предоставляет арендаторам возможность запускать реалистичные фишинговые атаки и учиться у них.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 56c0f8f8ce514e21b39e24494132ee6fec123d31
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979775"
---
# <a name="attacksimulationroot-resource-type"></a>тип ресурса attackSimulationRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет арендаторам возможность запускать реалистичные фишинговые атаки и учиться у них.
Это абстрактный тип.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Моделирование списка](../api/attacksimulationroot-list-simulations.md)|[коллекция моделирования](../resources/simulation.md)|Получите ресурсы моделирования из свойства навигации моделирования.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|моделирование|[коллекция моделирования](../resources/simulation.md)|Представляете кампанию моделирования атак и учебной кампании клиента.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attackSimulationRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationRoot"
}
```

