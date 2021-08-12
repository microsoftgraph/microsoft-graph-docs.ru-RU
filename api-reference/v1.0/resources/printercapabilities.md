---
title: тип printerCapabilities сложный
description: Представляет возможности, сообщаемые принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 530c67a3779caf2557c780f6c62446ab95164151f92a68ce6946ff86bfb0d8bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229061"
---
# <a name="printercapabilities-resource-type"></a>тип ресурса printerCapabilities

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет возможности, сообщаемые принтером или принтеромShare.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|contentTypes|Коллекция строк|Список поддерживаемых типов контента (MIME), поддерживаемых принтером. Не гарантируется, что служба универсальной печати поддерживает печать всех этих типов MIME.|
|isColorPrintingSupported|Логическое|True, если цветная печать поддерживается принтером; false в противном случае. Только для чтения.|
|feedOrientations|коллекция printerFeedOrientation|Список ориентаций каналов, поддерживаемых принтером.|
|isPageRangeSupported|Логическое|True, если принтер поддерживает печать по диапазонам страниц; false в противном случае.|
|качества|[коллекция printQuality](enums.md#printquality-values)|Свойства печати, поддерживаемые принтером.|
|dpis|Коллекция Int32|Список разрешений печати в DPI, поддерживаемых принтером.|
|duplexModes|[коллекция printDuplexMode](enums.md#printduplexmode-values)|Список режимов дуплекса, поддерживаемых принтером. Допустимые значения описаны в следующей таблице.|
|queueBufferSizeInBytes|Int32|Максимальный размер очереди задания печати, который может храниться на принтере.|
|copiesPerJob|[integerRange](integerrange.md)|Диапазон копий на одну работу, поддерживаемую принтером.|
|finishings|[коллекция printFinishing](enums.md#printfinishing-values)|Отделочные процессы, поддерживаемые принтером для печатного документа.|
|mediaColors|Коллекция строк|Средства массовой информации (например, бумажные) цвета, поддерживаемые принтером.|
|mediaTypes|Коллекция String|Типы мультимедиа, поддерживаемые принтером.|
|mediaSizes|Коллекция String|Размеры мультимедиа, поддерживаемые принтером. Поддерживает стандартные имена размеров для средств массовой информации ISO и ANSI. Допустимые значения находятся в следующей [таблице.](#mediasizes-values)|
|pagesPerSheet|Коллекция Int32|Поддерживаемое количество страниц ввода, которые необходимо навязать одному впечатлению.|
|ориентации|[коллекция printOrientation](enums.md#printorientation-values)|Ориентации печати, поддерживаемые принтером. Допустимые значения описаны в следующей таблице.|
|inputBins|Коллекция строк|Поддерживаемые ячейки ввода для принтера.|
|outputBins|Коллекция String|Поддерживаемые ячейки вывода принтера (лотки).|
|supportsFitPdfToPage|Логическое|True, если принтер поддерживает масштабирование страниц PDF в соответствие с размером печатных мультимедиа; false в противном случае.|
|multipageLayouts|[коллекция printMultipageLayout](enums.md#printmultipagelayout-values)|Направления презентации, поддерживаемые принтером. Поддерживаемые значения описаны в следующей таблице.|
|colorModes|[коллекция printColorMode](enums.md#printcolormode-values)|Цветовые режимы, поддерживаемые принтером. Допустимые значения описаны в следующей таблице.|
|topMargins|Коллекция Int32|Список поддерживаемых верхних полей (в микронах) для принтера.|
|bottomMargins|Коллекция Int32|Список поддерживаемых нижних полей (в микронах) для принтера.|
|rightMargins|Коллекция Int32|Список поддерживаемых правых полей (в микронах) для принтера.|
|leftMargins|Коллекция Int32|Список поддерживаемых левых полей (в микронах) для принтера.|
|разбор по копиям;|Логическое|True, если принтер поддерживает копирование при печати muliple копий многошагового документа; false в противном случае.|
|scalings|[коллекция printScaling](enums.md#printscaling-values)|Поддерживаемые масштабирования печати.|

### <a name="mediasizes-values"></a>mediaSizes values

|Значение|
|:---|
|A3|
|A4|
|A5|
|A6|
|JIS B4|
|JIS B5|
|JPN Hagaki|
|Северная Америка 5x7in|
|Северная Америка Executive|
|Письмо говермента Северной Америки|
|Индекс Северной Америки 3x5in|
|Индекс Северной Америки 4x8in|
|Индекс Северной Америки 5x8in|
|Счет в Северной Америке|
|Книги Северной Америки|
|Северная Америка Legal|
|Письмо Из Северной Америки|
|Фото l 3.5x5in|
|Визитная карточка|
|Photo|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerCapabilities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCapabilities",
  "contentTypes": [
    "String"
  ],
  "isColorPrintingSupported": "Boolean",
  "feedOrientations": [
    "String"
  ],
  "isPageRangeSupported": "Boolean",
  "qualities": [
    "String"
  ],
  "dpis": [
    "Integer"
  ],
  "duplexModes": [
    "String"
  ],
  "copiesPerJob": {
    "@odata.type": "microsoft.graph.integerRange"
  },
  "finishings": [
    "String"
  ],
  "mediaColors": [
    "String"
  ],
  "mediaTypes": [
    "String"
  ],
  "mediaSizes": [
    "String"
  ],
  "pagesPerSheet": [
    "Integer"
  ],
  "orientations": [
    "String"
  ],
  "outputBins": [
    "String"
  ],
  "supportsFitPdfToPage": "Boolean",
  "multipageLayouts": [
    "String"
  ],
  "colorModes": [
    "String"
  ],
  "inputBins": [
    "String"
  ],
  "topMargins": [
    "Integer"
  ],
  "bottomMargins": [
    "Integer"
  ],
  "rightMargins": [
    "Integer"
  ],
  "leftMargins": [
    "Integer"
  ],
  "collation": "Boolean",
  "scalings": [
    "String"
  ]
}
```

