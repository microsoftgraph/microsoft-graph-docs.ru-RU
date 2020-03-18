---
title: Тип ресурса windows81VpnProxyServer
description: VPN-прокси-сервер.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 345856eb5032026cd92c33cad07a620e3659f473
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786567"
---
# <a name="windows81vpnproxyserver-resource-type"></a>Тип ресурса windows81VpnProxyServer

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

VPN-прокси-сервер.


Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|аутоматикконфигуратионскриптурл|String|URL-адрес скрипта автоматической настройки прокси-сервера. Наследуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
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



