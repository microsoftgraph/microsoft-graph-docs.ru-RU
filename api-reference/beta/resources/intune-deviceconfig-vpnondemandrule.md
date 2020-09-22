---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aaa72419ce12195a042592abceb86ec754ea7341
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049032"
---
# <a name="vpnondemandrule-resource-type"></a>Тип ресурса Впнондемандруле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила VPN по запросу.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Идентификатор|Коллекция String|Идентификаторы набора сетевых служб (SSID).|
|днссеарчдомаинс|Коллекция String|Домены поиска DNS.|
|пробеурл|Строка|URL-адрес для зонда. Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.|
|action|[впнондемандрулеконнектионактион](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|Меры. Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.|
|домаинактион|[впнондемандрулеконнектиондомаинактион](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|Действие домена (применяется только при оценке подключения). Возможные значения: `connectIfNeeded`, `neverConnect`.|
|домена|Коллекция String|Домены (применяется только при оценке подключения).|
|проберекуиредурл|Строка|Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).|

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






