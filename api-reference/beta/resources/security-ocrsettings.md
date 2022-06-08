---
title: Тип ресурса ocrSettings
description: Параметры OCR для дела обнаружения электронных данных
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d3a72dbcbdf75abe0e2da50aa8626a828a4d2588
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946068"
---
# <a name="ocrsettings-resource-type"></a>Тип ресурса ocrSettings

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры OCR (оптическое распознавание символов) для дела обнаружения электронных данных.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включен ли OCR для дела.|
|maxImageSize|Int32|Максимальный размер образа, который будет обрабатываться в КБ).|
|timeout|Длительность|Длительность времени ожидания для обработчика OCR. Более длительное время ожидания может увеличить успешность OCR, но может увеличить общее время обработки.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.ocrSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```

