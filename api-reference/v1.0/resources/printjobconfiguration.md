---
title: тип ресурса printJobConfiguration
description: Группа параметров, которые принтер должен использовать для печати задания.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4fe417c8c2da43bc3378e15edac451619d2562a4
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944937"
---
# <a name="printjobconfiguration-resource-type"></a>тип ресурса printJobConfiguration

Пространство имен: microsoft.graph

Группа параметров, которые принтер должен использовать для печати задания.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|pageRanges|[коллекция integerRange](integerrange.md)|Страница колеблется для печати. Только для чтения.|
|качество|[printQuality](enums.md#printquality-values)|Качество печати, используемой при печати задания. Допустимые значения описаны в таблице ниже. Только для чтения.|
|dpi|Int32|Разрешение, используемого при печати задания, выраженного точками на дюйм (DPI). Только для чтения.|
|feedOrientation|printerFeedOrientation|Ориентация, используемая при подаче носителю в принтер. Допустимые значения описаны в следующей таблице. Только для чтения.|
|orientation|[printOrientation](enums.md#printorientation-values)|Параметр ориентации, который принтер должен использовать при печати задания. Допустимые значения описаны в следующей таблице.|
|duplexMode|[printDuplexMode](enums.md#printduplexmode-values)|Режим дуплекса, который принтер должен использовать при печати задания. Допустимые значения описаны в таблице ниже. Только для чтения.|
|копии|Int32|Количество копий, которые должны быть напечатаны. Только для чтения.|
|colorMode|[printColorMode](enums.md#printcolormode-values)|Цветовой режим, который принтер должен использовать для печати задания. Допустимые значения описаны в таблице ниже. Только для чтения.|
|inputBin|String|Ячейка ввода (лоток), используемая при печати. Сведения о возможностях [принтера см.](printercapabilities.md) в списке поддерживаемых корзин ввода.|
|outputBin|String|Ячейка вывода, в который можно разместить завершенные отпечатки. См. возможности [принтера для](printercapabilities.md) списка поддерживаемых бункеров выходных данных.|
|mediaSize|String|Размер мультимедиа, который необходимо использовать при печати. Поддерживает стандартные имена размеров для средств массовой информации ISO и ANSI. Допустимые значения, указанные в [разделе printerCapabilities.](printercapabilities.md#mediasizes-values)|
|margin|[printMargin](printmargin.md)|Параметры поля, которые необходимо использовать при печати.|
|MediaType|String|Тип мультимедиа по умолчанию (например, бумага) для печати документа.|
|finishings|[коллекция printFinishing](enums.md#printfinishing-values)|Отделочные процессы, которые необходимо использовать при печати.|
|pagesPerSheet|Int32|Количество страниц документов для печати на каждом листе.
|multipageLayout|[printMultipageLayout](enums.md#printmultipagelayout-values)|Направление для раскладывки страниц при печати нескольких страниц на один лист. Допустимые значения описаны в следующей таблице.|
|collate|Логическое|Должен ли принтер совмессировать страницы, печатая несколько копий много страниц документа.|
|масштабирование.|[printScaling](enums.md#printscaling-values)|Указывает, как принтер должен масштабировать данные документа, чтобы соответствовать запрашиваемой мультимедиа. Допустимые значения описаны в следующей таблице.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobConfiguration",
  "pageRanges": [
    {
      "@odata.type": "microsoft.graph.integerRange"
    }
  ],
  "quality": "String",
  "dpi": "Integer",
  "feedOrientation": "String",
  "orientation": "String",
  "duplexMode": "String",
  "copies": "Integer",
  "colorMode": "String",
  "inputBin": "String",
  "outputBin": "String",
  "mediaSize": "String",
  "margin": {
    "@odata.type": "microsoft.graph.printMargin"
  },
  "mediaType": "String",
  "finishings": [
    "String"
  ],
  "pagesPerSheet": "Integer",
  "multipageLayout": "String",
  "collate": "Boolean",
  "scaling": "String",
  "fitPdfToPage": "Boolean"
}
```

