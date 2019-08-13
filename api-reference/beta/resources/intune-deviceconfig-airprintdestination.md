---
title: Тип ресурса Аирпринтдестинатион
description: Представляет целевой объект Аирпринт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8e359e5df1ae55fdc50c42d98c2c5f44f8ea7dc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334943"
---
# <a name="airprintdestination-resource-type"></a>Тип ресурса Аирпринтдестинатион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет целевой объект Аирпринт.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ipAddress|String|IP-адрес назначения Аирпринт.|
|resourcePath|String|Путь к ресурсу, связанный с принтером. Соответствует параметру RP записи _ipps. TCP Бонжаур. Например: Printers/Canon_MG5300_series, Printers/Xerox_Phaser_7600, IPP/Print, Epson_IPP_Printer.|
|порта|Int32|Прослушивающий порт назначения Аирпринт. Если этот ключ не указан, Аирпринт будет использовать порт по умолчанию. Доступно в iOS 11,0 и более поздних версиях.|
|форцетлс|Boolean|Если задано значение true, подключения Аирпринт защищены с помощью протокола TLS. Значение по умолчанию — false. Доступно в iOS 11,0 и более поздних версиях.|

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



