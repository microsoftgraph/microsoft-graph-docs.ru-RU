---
title: Тип ресурса attackSimulationInfo
description: Представляет сведения об имитации атаки отправки угроз
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d7caee88f2d097c344c9fdcb3ba64767893e0276
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856782"
---
# <a name="attacksimulationinfo-resource-type"></a>Тип ресурса attackSimulationInfo

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об имитации атак отправки угроз. Если сообщение электронной почты было сообщением имитации атаки, отправка угрозы электронной почты будет содержать соответствующие сведения об имитации атаки.

## <a name="properties"></a>Свойства
| Свойство              | Тип           | Описание                          |
|:----------------------|:---------------|:-------------------------------------|
| attackSimDateTime     | DateTimeOffset | Указывает дату и время имитации атаки.   |
| attackSimDurationTime | Длительность       | Указывает длительность (во времени) моделирования атаки.  |
| attackSimId           | Guid           | Указывает идентификатор действия для имитации атаки. |
| attackSimUserId       | Строка         | Указывает идентификатор пользователя, который получил сообщение электронной почты для имитации атаки.   |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.attackSimulationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.attackSimulationInfo",
  "attackSimId": "Guid",
  "attackSimDateTime": "String (timestamp)",
  "attackSimDurationTime": "String (duration)",
  "attackSimUserId": "String"
}
```

