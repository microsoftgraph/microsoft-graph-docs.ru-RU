---
title: Тип ресурса windows81VpnProxyServer
description: VPN-прокси-сервер.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb4f94ee9cb1eabb76c5e0aead33ae323b05a8b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734261"
---
# <a name="windows81vpnproxyserver-resource-type"></a>Тип ресурса windows81VpnProxyServer

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

VPN-прокси-сервер.


Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|аутоматикконфигуратионскриптурл|Строка|URL-адрес скрипта автоматической настройки прокси-сервера. Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|Address. Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|порта|Int32|Порта. Допустимые значения — от 0 до 65535, наследуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|аутоматикаллидетектпроксисеттингс|Логический|Автоматически определять параметры прокси-сервера.|
|бипасспроксисерверфорлокаладдресс|Логический|Обход прокси-сервера для локального адреса.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```





