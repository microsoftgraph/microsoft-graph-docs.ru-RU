---
title: тип ресурса printerDefaults
description: Представляет параметры принтера по умолчанию. Проверьте возможности принтера, чтобы увидеть все поддерживаемые значения.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fbee453d42fbcb056ce3dce3ff7311e4d976b7dc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517343"
---
# <a name="printerdefaults-resource-type"></a>тип ресурса printerDefaults

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет параметры принтера по умолчанию. Проверьте возможности [принтера,](printercapabilities.md) чтобы увидеть все поддерживаемые значения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|copiesPerJob|Int32|Число экземпляров, напечатанных по умолчанию на одну работу.|
|contentType|String|Тип контента по умолчанию (MIME), который используется при обработке документов.|
|finishings|[коллекция printFinishing](enums.md#printfinishing-values)|Набор отделок по умолчанию, применимый к заданиям печати. Допустимые значения описаны в следующей таблице.|
|mediaColor|Строка|Цвет мультимедиа по умолчанию (например, бумажный) для печати документа.
|MediaType|Строка|Тип мультимедиа по умолчанию (например, бумага) для печати документа. Допустимые значения описаны в следующей таблице.|
|mediaSize|Строка|Размер мультимедиа по умолчанию, который необходимо использовать. Поддерживает стандартные имена размеров для средств массовой информации ISO и ANSI, а также любые настраиваемые размеры, поддерживаемые связанным принтером.
|pagesPerSheet|Int32|Число страниц документов по умолчанию для печати на каждом листе.
|orientation|[printOrientation](enums.md#printorientation-values)|Ориентация по умолчанию, используемая при печати документа. Допустимые значения описаны в следующей таблице.|
|outputBin|Строка|Ячейка вывода по умолчанию для того, чтобы разместить завершенные отпечатки. См. возможности [принтера для](printercapabilities.md) списка поддерживаемых бункеров выходных данных.|
|fitPdfToPage|Логический|Параметр fitPdfToPage по умолчанию. True, чтобы поместить каждую страницу документа PDF в физический лист мультимедиа; false, чтобы принтер решил, как выкладывать впечатления.|
|multipageLayout|[printMultipageLayout](enums.md#printmultipagelayout-values)|Направление по умолчанию для выкладки страниц при печати нескольких страниц на листе. Допустимые значения описаны в следующей таблице.|
|colorMode|[printColorMode](enums.md#printcolormode-values)|Цветной режим по умолчанию, который используется при печати документа. Допустимые значения описаны в следующей таблице.|
|качество|[printQuality](enums.md#printquality-values)|Качество по умолчанию, используемая при печати документа. Допустимые значения описаны в следующей таблице.|
|duplexMode|[printDuplexMode](enums.md#printduplexmode-values)|Двубоксовая конфигурация по умолчанию, используемая при печати документа. Допустимые значения описаны в следующей таблице.|
|dpi|Int32|Разрешение по умолчанию в DPI, используемом при печати задания.|
|scaling|[printScaling](enums.md#printscaling-values)|Указывает, как принтер масштабирует данные документа, чтобы соответствовать запрашиваемой мультимедиа. Допустимые значения описаны в следующей таблице.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerDefaults"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerDefaults",
  "copiesPerJob": "Integer",
  "contentType": "String",
  "finishings": [
    "String"
  ],
  "mediaColor": "String",
  "mediaType": "String",
  "mediaSize": "String",
  "pagesPerSheet": "Integer",
  "orientation": "String",
  "outputBin": "String",
  "inputBin": "String",
  "fitPdfToPage": "Boolean",
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String",
  "dpi": "Integer",
  "scaling": "String"
}
```

