---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa1ac8562ac2a43db43bb359cb189f8a4ed9500b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987581"
---
# <a name="vpnondemandrule-resource-type"></a>Тип ресурса Впнондемандруле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила VPN по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Идентификатор|Коллекция строк|Идентификаторы набора сетевых служб (SSID).|
|Днссеарчдомаинс|Коллекция строк|Домены поиска DNS.|
|Пробеурл|String|URL-адрес для зонда. Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.|
|action|[Впнондемандрулеконнектионактион](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Меры. Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|Домаинактион|[Впнондемандрулеконнектиондомаинактион](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Действие домена (применяется только при оценке подключения). Возможные значения: `connectIfNeeded`, `neverConnect`.|
|домена|Коллекция строк|Домены (применяется только при оценке подключения).|
|Проберекуиредурл|String|Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```





