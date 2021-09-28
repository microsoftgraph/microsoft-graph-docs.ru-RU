---
title: тип ресурса userSimulationEventInfo
description: Представляет событие моделирования пользователя в клиенте в кампании моделирования атак и обучения.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 423eb3f5f15d4730d1229febde71aec9930ff81f
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979704"
---
# <a name="usersimulationeventinfo-resource-type"></a>тип ресурса userSimulationEventInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет событие моделирования пользователя в клиенте в кампании моделирования атак и обучения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Обозреватель|Строка|Сведения браузера, из которых событие моделирования было инициировано пользователем в кампании моделирования атак и обучения.|
|eventDateTime|DateTimeOffset|Дата и время события моделирования пользователем в кампании моделирования атак и учебной кампании.|
|eventName|Строка|Имя события моделирования пользователем в кампании моделирования атак и учебной кампании.|
|ipAddress|String|IP-адрес, с которых событие моделирования было инициировано пользователем в кампании моделирования атак и обучения.|
|osPlatformDeviceDetails|Строка|Сведения об операционной системе, платформе и устройстве, с которых событие моделирования было инициировано пользователем в кампании моделирования атак и обучения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSimulationEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSimulationEventInfo",
  "eventName": "String",
  "eventDateTime": "String (timestamp)",
  "ipAddress": "String",
  "osPlatformDeviceDetails": "String",
  "browser": "String"
}
```

