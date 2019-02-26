---
title: Тип ресурса windows10VpnProxyServer
description: VPN-прокси-сервер.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4686049e2f3525409e81ec1492dcb052ab9f3657
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140693"
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
|port|Int32|Порта. Допустимые значения — от 0 до 65535, наСледуемые от [впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|
|Бипасспроксисерверфорлокаладдресс|Логический|Обход прокси-сервера для локального адреса.|

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




