---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdb362bcbf672f491e22e2ee7d69a7e5c243e812
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944616"
---
# <a name="vpndnsrule-resource-type"></a>Тип ресурса Впнднсруле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение правила DNS для VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|String|Расширением.|
|серверами|Коллекция строк|Серверами.|
|Проксисерверури|Строка|URI прокси-сервера.|
|автотриггер|Логический|Автоматически подключаться к ВИРТУАЛЬНОЙ частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.|
|сохраняемого|Логический|Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.|

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




