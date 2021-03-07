---
title: тип printerCapabilities сложный
description: Представляет возможности, сообщаемые принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5416cf43e266bab65254ac5aaee1a79c9c3e17be
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517338"
---
# <a name="printercapabilities-resource-type"></a>тип ресурса printerCapabilities

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Представляет возможности, сообщаемые принтером или принтеромShare.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|contentTypes|Коллекция строк|Список поддерживаемых типов контента (MIME), поддерживаемых принтером. Не гарантируется, что служба универсальной печати поддерживает печать всех этих типов MIME.|
|isColorPrintingSupported|Логический|True, если цветная печать поддерживается принтером; false в противном случае. Только для чтения.|
|feedOrientations|коллекция printerFeedOrientation|Список ориентаций каналов, поддерживаемых принтером.|
|isPageRangeSupported|Логический|True, если принтер поддерживает печать по диапазонам страниц; false в противном случае.|
|качества|[коллекция printQuality](enums.md#printquality-values)|Свойства печати, поддерживаемые принтером.|
|dpis|Коллекция Int32|Список разрешений печати в DPI, поддерживаемых принтером.|
|duplexModes|[коллекция printDuplexMode](enums.md#printduplexmode-values)|Список режимов дуплекса, поддерживаемых принтером. Допустимые значения описаны в следующей таблице.|
|queueBufferSizeInBytes|Int32|Максимальный размер очереди задания печати, который может храниться на принтере.|
|copiesPerJob|[integerRange](integerrange.md)|Диапазон копий на одну работу, поддерживаемую принтером.|
|finishings|[коллекция printFinishing](enums.md#printfinishing-values)|Отделочные процессы, поддерживаемые принтером для печатного документа.|
|mediaColors|Коллекция строк|Средства массовой информации (например, бумажные) цвета, поддерживаемые принтером.|
|mediaTypes|Коллекция строк|Типы мультимедиа, поддерживаемые принтером. Допустимые значения описаны в следующей таблице.|
|mediaSizes|Коллекция строк|Размеры мультимедиа, поддерживаемые принтером. Поддерживает стандартные имена размеров для средств массовой информации ISO и ANSI, а также любые настраиваемые размеры, поддерживаемые связанным принтером.|
|pagesPerSheet|Коллекция Int32|Поддерживаемое количество страниц ввода, которые необходимо навязать одному впечатлению.|
|ориентации|[коллекция printOrientation](enums.md#printorientation-values)|Ориентации печати, поддерживаемые принтером. Допустимые значения описаны в следующей таблице.|
|inputBins|Коллекция строк|Поддерживаемые ячейки ввода для принтера.|
|outputBins|Коллекция строк|Поддерживаемые ячейки вывода принтера (лотки).|
|supportsFitPdfToPage|Логический|True, если принтер поддерживает масштабирование страниц PDF в соответствие с размером печатных мультимедиа; false в противном случае.|
|multipageLayouts|[коллекция printMultipageLayout](enums.md#printmultipagelayout-values)|Направления презентации, поддерживаемые принтером. Поддерживаемые значения описаны в следующей таблице.|
|colorModes|[коллекция printColorMode](enums.md#printcolormode-values)|Цветовые режимы, поддерживаемые принтером. Допустимые значения описаны в следующей таблице.|
|topMargins|Коллекция Int32|Список поддерживаемых верхних полей (в микронах) для принтера.|
|bottomMargins|Коллекция Int32|Список поддерживаемых нижних полей (в микронах) для принтера.|
|rightMargins|Коллекция Int32|Список поддерживаемых правых полей (в микронах) для принтера.|
|leftMargins|Коллекция Int32|Список поддерживаемых левых полей (в микронах) для принтера.|
|collation|Логический|True, если принтер поддерживает копирование при печати muliple копий многошагового документа; false в противном случае.|
|scalings|[коллекция printScaling](enums.md#printscaling-values)|Поддерживаемые масштабирования печати.|

## <a name="relationships"></a>Отношения
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

