---
title: тип ресурса airPrintDestination
description: Представляет пункт назначения AirPrint.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad603ab29c7914ccb16845ceeddda89581a40568
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095697"
---
# <a name="airprintdestination-resource-type"></a>тип ресурса airPrintDestination

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет пункт назначения AirPrint.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ipAddress|String|IP-адрес назначения AirPrint.|
|resourcePath|String|Путь ресурсов, связанный с принтером. Это соответствует параметру RP записи _ipps.tcp Bonjour. Например: принтеры/Canon_MG5300_series, принтеры/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.|
|порт|Int32|Порт прослушивания назначения AirPrint. Если этот ключ не указан, AirPrint будет использовать порт по умолчанию. Доступна в iOS 11.0 и более поздней.|
|forceTls|Логическое|Если верное подключение AirPrint обеспечивается безопасностью транспортного слоя (TLS). Значение по умолчанию: false. Доступна в iOS 11.0 и более поздней.|

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



