---
title: Тип ресурса windows10VpnProxyServer
description: VPN-прокси-сервер.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 212bafa99a51e269716978cafa4fcf274dd76579
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797902"
---
# <a name="windows10vpnproxyserver-resource-type"></a>Тип ресурса windows10VpnProxyServer

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

VPN-прокси-сервер.


НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Аутоматикконфигуратионскриптурл|String|URL-адрес скрипта автоматической настройки прокси-сервера. НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|address|String|Address. НаСледуется от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|порта|Int32|Порта. Допустимые значения — от 0 до 65535, наСледуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|Бипасспроксисерверфорлокаладдресс|Boolean|Обход прокси-сервера для локального адреса.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```





