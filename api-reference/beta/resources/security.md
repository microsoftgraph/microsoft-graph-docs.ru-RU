---
title: тип ресурсов безопасности
description: Подключение продуктов, служб и партнеров майкрософт для оптимизации операций по обеспечению безопасности и улучшения возможностей защиты от угроз, обнаружения и реагирования.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9f4640acb574c5099d0c1e928452099047f9cc71
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979803"
---
# <a name="security-resource-type"></a>тип ресурсов безопасности

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подключение продуктов, служб и партнеров майкрософт для оптимизации операций по обеспечению безопасности и улучшения возможностей защиты от угроз, обнаружения и реагирования.

## <a name="methods"></a>Методы
Нет.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|оповещения|Коллекция [alert](../resources/alert.md)|Уведомления о подозрительных или потенциальных проблемах безопасности клиента.|
|attackSimulation|[attackSimulationRoot](../resources/attacksimulationroot.md)|Предоставляет арендаторам возможность запускать смоделированную и реалистичную фишинговую атаку и учиться у нее.|
|securityactions|[securityAction](../resources/securityaction.md)|Действия, которые реагируют на оповещения для блокировки вредоносных действий.|
|tiindicators|[коллекция tiIndicator](../resources/tiindicator.md)|Индикаторы угроз, отправленные в Корпорацию Майкрософт, которые определяют вредоносные действия.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security"
}
```

