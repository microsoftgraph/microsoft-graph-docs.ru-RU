---
title: Тип ресурса airPrintDestination
description: Представляет целевой объект AirPrint.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422497"
---
# <a name="airprintdestination-resource-type"></a>Тип ресурса airPrintDestination

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет целевой объект AirPrint.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ipAddress|String|IP-адрес назначения AirPrint.|
|resourcePath|String|Путь к ресурсу, связанных с принтером. Это соответствует параметру rp _ipps.tcp Bonjour записи. Например: принтеры/Canon_MG5300_series, принтеры/Xerox_Phaser_7600, ipp/print Epson_IPP_Printer.|
|port|Int32|Прослушивающий порт назначения AirPrint. Если этот ключ не указан AirPrint будет использовать порт по умолчанию. Доступные в iOS 11.0 и более поздних версий.|
|forceTls|Логический|Если значение true, AirPrint подключения будут защищены по безопасности TLS (Transport Layer). Значение по умолчанию — false. Доступные в iOS 11.0 и более поздних версий.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```




