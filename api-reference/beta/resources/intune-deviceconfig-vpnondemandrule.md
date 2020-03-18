---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cb1274dd966553ecde0514e0603619b6ed803c77
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787364"
---
# <a name="vpnondemandrule-resource-type"></a>Тип ресурса Впнондемандруле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила VPN по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Идентификатор|Коллекция String|Идентификаторы набора сетевых служб (SSID).|
|днссеарчдомаинс|Коллекция String|Домены поиска DNS.|
|пробеурл|String|URL-адрес для зонда. Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.|
|action|[впнондемандрулеконнектионактион](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Меры. Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|домаинактион|[впнондемандрулеконнектиондомаинактион](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Действие домена (применяется только при оценке подключения). Возможные значения: `connectIfNeeded`, `neverConnect`.|
|домена|Коллекция String|Домены (применяется только при оценке подключения).|
|проберекуиредурл|String|Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).|

## <a name="relationships"></a>Связи
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



