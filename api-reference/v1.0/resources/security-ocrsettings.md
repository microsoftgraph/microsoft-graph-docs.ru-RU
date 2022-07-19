---
title: Тип ресурса ocrSettings
description: Представляет параметры OCR для дела обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d4b15f7bef89c37f4debedb58ed48734f86b1bef
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839645"
---
# <a name="ocrsettings-resource-type"></a>Тип ресурса ocrSettings

Пространство имен: microsoft.graph.security



Представляет параметры оптического распознавания символов (OCR) для дела обнаружения электронных данных.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включен ли OCR для дела.|
|maxImageSize|Int32|Максимальный размер образа, который будет обрабатываться в КБ).|
|timeout|Длительность|Длительность времени ожидания для обработчика OCR. Более длительное время ожидания может увеличить успешность OCR, но может увеличить общее время обработки.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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

