---
title: тип ресурса attackSimulationRoot
description: Предоставляет возможность запуска реалистичной фишинговой атаки, на которую организации могут извлечь уроки.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b83d13c6541b036bf3096f6ba6e99a9f4dfb79f5
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757672"
---
# <a name="attacksimulationroot-resource-type"></a>тип ресурса attackSimulationRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет возможность запуска реалистичной фишинговой атаки, на которую организации могут извлечь уроки.
Это абстрактный тип.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление симуляций](../api/attacksimulationroot-list-simulations.md)|[коллекция моделирования](../resources/simulation.md)|Получите список обучающих кампаний по имитации атак для клиента.|
|[Моделирование спискаАтомации](../api/attacksimulationroot-list-simulationautomations.md)|[коллекция simulationAutomation](../resources/simulationautomation.md)|Получите список автоматизации моделирования атак для клиента.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|моделирование|[коллекция моделирования](../resources/simulation.md)|Представляет обучающую кампанию по имитации атак в клиенте.|
|simulationAutomations|[коллекция simulationAutomation](../resources/simulationautomation.md)|Представляет автоматизацию моделирования, созданную для работы с клиентом.|

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

