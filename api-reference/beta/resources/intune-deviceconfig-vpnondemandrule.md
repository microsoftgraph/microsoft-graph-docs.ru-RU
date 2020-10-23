---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8429cb0a7870cb1ee756f5e2c02b218d5c768862
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728351"
---
# <a name="vpnondemandrule-resource-type"></a>Тип ресурса Впнондемандруле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила VPN по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Идентификатор|Коллекция строк|Идентификаторы набора сетевых служб (SSID).|
|днссеарчдомаинс|Коллекция строк|Домены поиска DNS.|
|пробеурл|Строка|URL-адрес для зонда. Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.|
|action|[впнондемандрулеконнектионактион](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Меры. Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|домаинактион|[впнондемандрулеконнектиондомаинактион](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Действие домена (применяется только при оценке подключения). Возможные значения: `connectIfNeeded`, `neverConnect`.|
|домена|Коллекция строк|Домены (применяется только при оценке подключения).|
|проберекуиредурл|Строка|Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).|

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





