---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8d3f9349d7b966a608aaa1b0bef04b00df6a475f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049110"
---
# <a name="vpndnsrule-resource-type"></a>Тип ресурса Впнднсруле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила DNS для VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Расширением.|
|серверами|Коллекция String|Серверами.|
|проксисерверури|Строка|URI прокси-сервера.|
|автотриггер|Boolean|Автоматически подключаться к виртуальной частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.|
|сохраняемого|Boolean|Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```






