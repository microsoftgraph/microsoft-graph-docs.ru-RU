---
title: Тип ресурса Впнднсруле
description: Определение правила DNS для VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 983b30b1f724c3c8f76e967179c6fcdb1ff1fecb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367731"
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
|проксисерверури|String|URI прокси-сервера.|
|автотриггер|Boolean|Автоматически подключаться к виртуальной частной сети, когда устройство подключается к этому домену: значение по умолчанию — false.|
|сохраняемого|Boolean|Оставить это правило активным, даже если VPN-подключение не подключено: по умолчанию используется значение false.|

## <a name="relationships"></a>Отношения
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



