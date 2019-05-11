---
title: Тип ресурса Аирпринтдестинатион
description: Представляет целевой объект Аирпринт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90eb7d01afacf65e96623fea35128c122e55d16b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949222"
---
# <a name="airprintdestination-resource-type"></a>Тип ресурса Аирпринтдестинатион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет целевой объект Аирпринт.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ipAddress|String|IP-адрес назначения Аирпринт.|
|resourcePath|Строка|Путь к ресурсу, связанный с принтером. Соответствует параметру RP записи _иппс. TCP Бонжаур. Например: Printers/Canon_MG5300_series, Printers/Xerox_Phaser_7600, IPP/Print, Епсон_ипп_принтер.|
|порта|Int32|Прослушивающий порт назначения Аирпринт. Если этот ключ не указан, Аирпринт будет использовать порт по умолчанию. Доступно в iOS 11,0 и более поздних версиях.|
|Форцетлс|Логический|Если задано значение true, подключения Аирпринт защищены с помощью протокола TLS. Значение по умолчанию — false. Доступно в iOS 11,0 и более поздних версиях.|

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




