---
title: Тип ресурса ocrSettings
description: Представляет параметры OCR для дела обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e3951812e8196a4bd5839f5580cf79bac8bc671e
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838229"
---
# <a name="ocrsettings-resource-type"></a>Тип ресурса ocrSettings

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

