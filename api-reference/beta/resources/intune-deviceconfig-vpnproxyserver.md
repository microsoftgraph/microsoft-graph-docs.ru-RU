---
title: Тип ресурса Впнпроксисервер
description: VPN-прокси-сервер.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b004eaae0b49c9f3e4341c32923d7f2d48ae45
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944581"
---
# <a name="vpnproxyserver-resource-type"></a>Тип ресурса Впнпроксисервер

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

VPN-прокси-сервер.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Аутоматикконфигуратионскриптурл|Строка|URL-адрес скрипта автоматической настройки прокси-сервера.|
|address|String|Address.|
|порта|Int32|Порта. Допустимые значения — от 0 до 65535|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```




