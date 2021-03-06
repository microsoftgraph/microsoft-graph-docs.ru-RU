---
title: Тип ресурса printerDefaults
description: Представляет параметры принтера по умолчанию. Проверьте возможности принтера, чтобы увидеть все поддерживаемые значения.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7121760cc823470a0ea7b64e57cab8f61b231be8
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292618"
---
# <a name="printerdefaults-resource-type"></a>Тип ресурса printerDefaults

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры принтера по умолчанию. Проверьте возможности [принтера,](printercapabilities.md) чтобы увидеть все поддерживаемые значения.

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|copiesPerJob|Int32|Количество печатаемой копии по умолчанию для каждого задания.|
|contentType|String|Тип контента по умолчанию (MIME), который будет применяться при обработке документов.|
|finishings|Коллекция printFinishing|Набор завершений по умолчанию, которые применяются к заданиям печати. Допустимые значения описаны в следующей таблице.|
|mediaColor|String|Цвет мультимедиа по умолчанию (например, бумага) для печати документа.
|MediaType|String|Тип мультимедиа по умолчанию (например, бумага) для печати документа. Допустимые значения описаны в следующей таблице.|
|mediaSize|String|Размер мультимедиа по умолчанию для использования. Поддерживает имена стандартных размеров для размеров мультимедиа ISO и ANSI, а также любые пользовательские размеры, поддерживаемые связанным принтером.
|pagesPerSheet|Int32|Количество страниц документов по умолчанию для печати на каждом листе.
|orientation|printOrientation|Ориентация по умолчанию, используемая при печати документа. Допустимые значения описаны в следующей таблице.|
|inputBin|String|Корзина ввода по умолчанию, которая выступает в качестве источника бумаги.|
|outputBin|String|Корзина вывода по умолчанию, в которая необходимо разместить завершенные печати. Список поддерживаемых выходных [контейнеров](printercapabilities.md) см. в возможностях принтера.|
|fitPdfToPage|Логический|Параметр fitPdfToPage по умолчанию. True, чтобы поместить каждую страницу PDF-документа на физический лист мультимедиа; false, чтобы принтер решил, как разложить показы.|
|multipageLayout|printMultipageLayout|Направление по умолчанию для настройки страниц, когда на листе печатается несколько страниц. Допустимые значения описаны в следующей таблице.|
|colorMode|printColorMode|Цветовой режим по умолчанию, который будет применяться при печати документа. Допустимые значения описаны в следующей таблице.|
|quality|printQuality|Качество по умолчанию, используемая при печати документа. Допустимые значения описаны в следующей таблице.|
|duplexMode|printDuplexMode|Конфигурация duplex по умолчанию (с двух стороной), используемая при печати документа. Допустимые значения описаны в следующей таблице.|
|dpi|Int32|Разрешение по умолчанию в DPI, используемом при печати задания.|
|scaling|printScaling|Указывает, как принтер масштабирует данные документа в нужном мультимедиа. Допустимые значения описаны в следующей таблице.|

### <a name="printmultipagelayout-values"></a>Значения printMultipageLayout

|Элемент|Значение|Описание|
|:---|:---|:---|
|clockwiseFromTopLeft|0|Расположите страницы в сетке по часовой стрелке, начиная с левого верхнего.|
|counterClockwiseFromTopLeft|1 |Расположите страницы в сетке против часовой стрелки, начиная с левого верхнего.|
|counterClockwiseFromTopRight|2 |Расположите страницы в сетке против часовой стрелки, начиная с верхнего правого.|
|clockwiseFromTopRight|3 |Расположите страницы в сетке по часовой стрелке, начиная с верхнего правого.|
|counterClockwiseFromBottomLeft|4 |Расположите страницы в сетке против часовой стрелки, начиная с левого нижнего.|
|clockwiseFromBottomLeft|5 |Расположите страницы в сетке по часовой стрелке, начиная с нижнего левого.|
|counterClockwiseFromBottomRight|6 |Расположите страницы в сетке против часовой стрелки, начиная с нижнего правого.|
|clockwiseFromBottomRight|7 |Расположите страницы в сетке по часовой стрелке, начиная с нижнего правого.|

### <a name="printduplexmode-values"></a>значения printDuplexMode

|Элемент|Значение|Описание|
|:---|:---|:---|
|flipOnLongEdge|0|Принтер напечатает две стороны и будет пролистывать документы вдоль длинного края.|
|flipOnShortEdge|1 |Принтер напечатает две стороны и будет пролистывать документы вдоль короткого края.|
|oneSided|2 |Принтер напечатает однобокий принтер.|

### <a name="printfinishing-values"></a>значения printFinishing

|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|3 |Завершение не заканчивается. Включив это значение, можно предоставить пустую коллекцию завершений.|
|365|4 |Скрепить документ, используя стандартную конфигурацию затухания принтера.|
|1|5 |Ветвь документа с помощью конфигурации с затухаемой по умолчанию конфигурацией принтера.|
|cover|6 |Применив к документу обложку.|
|bind|7 |Привяжете документ с помощью конфигурации привязки принтера по умолчанию.|
|itchStitch|8 |Запечатав документ с использованием конфигурации настройки по умолчанию для принтера.|
|edge|9 |Обустройка по краям документа с использованием конфигурации настроек принтера по умолчанию.|
|stapleTopLeft|20|Скрепить документ в верхнем левом углу.|
|botBottomLeft|21|Скрепить документ в левом нижнем углу.|
|stapleTopRight|22|Скрепить документ в правом верхнем углу.|
|botBottomRight|23|Скрепить документ в правом нижнем углу.|
|stitchLeftEdge|24|По краям выстройте документ вдоль левого края.|
|stitchTopEdge|25|По краям выстройте документ вдоль верхнего края.|
|stitchRightEdge|26|По краям выстройте документ вдоль правого края.|
|botBottomEdge|27|По краям выстройте документ вдоль нижнего края.|
|stapleDualLeft|28|Дважды скрепить документ вдоль левого края.|
|stapleDualTop|29|Скрепить документ дважды вдоль верхнего края.|
|stapleDualRight|30|Скрепить документ дважды вдоль правого края.|
|stapleDualBottom|31|Скрепить документ дважды вдоль нижнего края.|
|unknownFutureValue|32|Постоянно меняющееся значение sentinel для enumeration. Не следует использовать.|

## <a name="printorientation-values"></a>значения printOrientation

|Элемент|Значение|Описание|
|:---|:---|:---|
|кивная|3 |Принтер будет печатать показы в "кантной" ориентации.|
|альбомная|4 |Принтер будет печатать показы в "альбомной" ориентации.|
|reverseLandscape|5 |Принтер будет печатать показы в "обратной альбомной" ориентации.|
|reversePortrait|6 |Принтер будет печатать показы в ориентации "обратного кисть".|

### <a name="printquality-values"></a>значения printQuality

|Элемент|Значение|Описание|
|:---|:---|
|low|0|Принтер напечатает задание, используя низкое качество (обычное название — черновик).|
|medium|1 |Принтер напечатает задание с помощью medim (обычного) качества.|
|high|2 |Принтер напечатает задание с использованием высокого (обычно известного как "лучшее" или "отличное") качества.|
|unknownFutureValue|3 |Постоянно меняющееся значение sentinel для enumeration. Не следует использовать.|

### <a name="printcolormode-values"></a>Значения printColorMode

|Элемент|Значение|Описание|
|:---|:---|:---|
|blackAndWhite|0|Черно-белый (используйте только материал черного маркера).)|
|grayscale|1 |Серый (может использовать какой-то материал цветового маркера).)|
|color|2 |Цвет (используйте любое сочетание материалов маркера для создания цветового впечатления).|
|Авто|3 |Разрешим принтеру выбрать цветной режим.|

### <a name="printscaling-values"></a>значения printScaling

|Элемент|Значение|Описание|
|:---|:---|:---|
|Авто|0|Если размер документа превышает запрашиваемого носителю, а поля ненулевые, принтер  масштабирования документа соответствует размеру printScaling. В противном случае принтер масштабирования документа с помощью **заливки** printScaling. Если размер документа меньше запрашиваемой, используется printScaling "none".|
|shrinkToFit|1 |Если размер документа превышает размер запрашиваемого носителя, принтер  масштабирования документа соответствует размеру printScaling. В противном случае принтер масштабирования документа, как **не** printScaling.|
|fill|2 |Принтер масштабирования документа для заполнения запрашиваемого размера мультимедиа, сохраняя пропорции, но потенциально обрезки части документа.|
|fit|3 |Принтер масштабирования документа в зависимости от области для печати запрашиваемого размера мультимедиа, сохраняя пропорции данных документа без обрезки документа.|
|Нет|4 |Принтер не масштабировать документ в зависимости от размера запрашиваемого носителя. Если размер документа превышает запрашиваемую, принтер центрировать и обрезает итоговые выходные данные. Если размер документа меньше, чем у запрашиваемного носителя, принтер выводит по центру.|
|unknownFutureValue|5 |Постоянно меняющееся значение sentinel для enumeration. Не следует использовать.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerDefaults"
}-->

```json
{
  "copiesPerJob": 123456,
  "contentType": "String",
  "finishings": ["String"],
  "mediaColor": "String",
  "mediaSize": "String",
  "pagesPerSheet": 123456,
  "orientation": "String",
  "outputBin": "String",
  "fitPdfToPage": true,
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String"
}

```

## <a name="see-also"></a>См. также

* [restoreFactoryDefaults](../api/printer-restorefactorydefaults.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerDefaults resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

