---
title: Тип ресурса vpnProxyServer
description: VPN-сервер прокси-сервера.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 727d26af7f2c1801cd06fc98949109efec267f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955354"
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





