---
title: Тип ресурса airPrintDestination
description: Представляет целевой объект AirPrint.
author: tfitzmac
ms.openlocfilehash: 046f85c65d382b34e6920f30f6b2718f817371a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361056"
---
# <a name="airprintdestination-resource-type"></a>Тип ресурса airPrintDestination

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет целевой объект AirPrint.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ipAddress|String|IP-адрес назначения AirPrint.|
|resourcePath|String.|Путь к ресурсу, связанных с принтером. Это соответствует параметру rp _ipps.tcp Bonjour записи. Например: принтеры/Canon_MG5300_series, принтеры/Xerox_Phaser_7600, ipp/print Epson_IPP_Printer.|
|port|Int32|Прослушивающий порт назначения AirPrint. Если этот ключ не указан AirPrint будет использовать порт по умолчанию. Доступные в iOS 11.0 и более поздних версий.|
|forceTls|Boolean.|Если значение true, AirPrint подключения будут защищены по безопасности TLS (Transport Layer). Значение по умолчанию — false. Доступные в iOS 11.0 и более поздних версий.|

## <a name="relationships"></a>Связи
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





