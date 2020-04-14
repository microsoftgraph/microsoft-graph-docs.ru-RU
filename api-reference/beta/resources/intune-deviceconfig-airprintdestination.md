---
title: Тип ресурса Аирпринтдестинатион
description: Представляет целевой объект Аирпринт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a89415cfaf2555d870c2f2ebb552776fd7720e4f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470973"
---
# <a name="airprintdestination-resource-type"></a>Тип ресурса Аирпринтдестинатион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет целевой объект Аирпринт.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ipAddress|String|IP-адрес назначения Аирпринт.|
|resourcePath|String|Путь к ресурсу, связанный с принтером. Соответствует _ipps параметру RP записи Бонжаур. TCP. Например: Printers/Canon_MG5300_series, Printers/Xerox_Phaser_7600, IPP/Print, Epson_IPP_Printer.|
|порта|Int32|Прослушивающий порт назначения Аирпринт. Если этот ключ не указан, Аирпринт будет использовать порт по умолчанию. Доступно в iOS 11,0 и более поздних версиях.|
|форцетлс|Boolean|Если задано значение true, подключения Аирпринт защищены с помощью протокола TLS. Значение по умолчанию: false. Доступно в iOS 11,0 и более поздних версиях.|

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



