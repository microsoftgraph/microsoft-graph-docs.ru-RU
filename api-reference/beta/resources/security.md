---
title: тип ресурсов безопасности
description: Подключение продуктов, служб и партнеров майкрософт для оптимизации операций по обеспечению безопасности и улучшения возможностей защиты от угроз, обнаружения и реагирования.
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 494fc483645fe0a5422013556b2a44cc21aaadaf
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220768"
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
|инциденты | [коллекция инцидентов](incident.md) | Коллекция инцидентов в Microsoft 365 Defender, каждый из которых — набор коррелирующих оповещений и связанных метаданных, отражающих историю атаки.|
|secureScores | [коллекция secureScore](securescores.md) | Измерения позы безопасности клиентов, чтобы защитить их от угроз. |
|securityactions|[коллекция securityAction](../resources/securityaction.md)|Действия, которые реагируют на оповещения для блокировки вредоносных действий.|
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

