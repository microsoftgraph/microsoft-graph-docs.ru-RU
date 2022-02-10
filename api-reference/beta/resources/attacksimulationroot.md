---
title: тип ресурса attackSimulationRoot
description: Предоставляет арендаторам возможность запускать реалистичные фишинговые атаки и учиться у них.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e38107d7c6d95706508ea5260fa9e88c87774672
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519742"
---
# <a name="attacksimulationroot-resource-type"></a>тип ресурса attackSimulationRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет арендаторам возможность запускать реалистичные фишинговые атаки и учиться у них.
Это абстрактный тип.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление симуляций](../api/attacksimulationroot-list-simulations.md)|[коллекция моделирования](../resources/simulation.md)|Получите ресурсы моделирования из свойства навигации моделирования.|

## <a name="properties"></a>Свойства
Нет

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

