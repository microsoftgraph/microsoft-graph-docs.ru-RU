---
title: Тип ресурса vpnProxyServer
description: VPN-сервер прокси-сервера.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b4842444bc248e51e1967fcbef4a863ed50498c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867678"
---
# <a name="vpnproxyserver-resource-type"></a>Тип ресурса vpnProxyServer

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

VPN-сервер прокси-сервера.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|automaticConfigurationScriptUrl|Строка|Прокси-Автоматическая настройка сценария URL-адрес.|
|address|String|Адрес.|
|port|Int32|Порт. Допустимые значения от 0 до 65535|

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





