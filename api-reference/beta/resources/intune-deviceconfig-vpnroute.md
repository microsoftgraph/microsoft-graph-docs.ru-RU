---
title: Тип ресурса Впнрауте
description: Определение маршрута VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54706d47267eef8fff6c465f24e4e9caa183ccc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154301"
---
# <a name="vpnroute-resource-type"></a>Тип ресурса Впнрауте

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение маршрута VPN.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Дестинатионпрефикс|String|Префикс назначения (IPv4/V6-адрес).|
|Префикссизе|Int32|Размер префикса. (1-32). Допустимые значения — от 1 до 32|

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




