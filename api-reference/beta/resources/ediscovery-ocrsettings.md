---
title: тип ресурса ocrSettings
description: Параметры OCR для дела об обнаружении электронной почты
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 648e0ad63f558f211591d1c8aa976c2689dd271d
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080893"
---
# <a name="ocrsettings-resource-type"></a>тип ресурса ocrSettings

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры OCR (Optical Character Recognition) для дела об обнаружении электронных обнаружений.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включен ли OCR для дела.|
|maxImageSize|Int32|Максимальный размер изображения, который будет обрабатываться в КБ).|
|timeout|Duration|Продолжительность периода времени для двигателя OCR. Более длительный период времени может повысить успешность OCR, но может увеличить общее время обработки.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```
