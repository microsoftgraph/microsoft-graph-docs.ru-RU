---
title: Тип ресурса vpnRoute
description: Определение маршрута VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 628e2f384b06dece13da1595a4111a2d1022a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423022"
---
# <a name="vpnroute-resource-type"></a>Тип ресурса vpnRoute

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение маршрута VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|destinationPrefix|String|Префикс назначения (адрес IPv4/v6).|
|prefixSize|Int32|Префикс размера. (1-32). Допустимые значения 1 до 32|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```




