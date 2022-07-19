---
title: Тип ресурса security
description: Подключает продукты, службы и партнеры майкрософт для упрощения операций безопасности и улучшения защиты от угроз, обнаружения и реагирования.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c7342f83c64b895b08a66429e0e20ab2cd7b5960
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856290"
---
# <a name="security-resource-type"></a>Тип ресурса security

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подключает продукты, службы и партнеры майкрософт для упрощения операций безопасности и улучшения защиты от угроз, обнаружения и реагирования.

## <a name="methods"></a>Методы
Нет.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|оповещения|Коллекция [alert](../resources/alert.md)|Уведомления о подозрительных или потенциальных проблемах безопасности в клиенте клиента.|
|attackSimulation|[attackSimulationRoot](../resources/attacksimulationroot.md)|Предоставляет клиентам возможность запускать имитацию и реалистичные фишинговые атаки и учиться на них.|
|securityactions|[securityAction](../resources/securityaction.md)|Действия, которые реагируют на оповещения для блокировки вредоносных действий.|
|tiindicators|[Коллекция tiIndicator](../resources/tiindicator.md)|Индикаторы угроз, отправляемые в корпорацию Майкрософт, которые идентифицируют вредоносные действия.|
|threatSubmission|[security.threatSubmission](../resources/security-threatsubmission.md)|Отправка угрозы в корпорацию Майкрософт; Например, подозрительная угроза электронной почты, угроза URL-адреса или файловая угроза.|

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

