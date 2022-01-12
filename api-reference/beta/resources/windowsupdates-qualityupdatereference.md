---
title: тип ресурса qualityUpdateReference
description: Представляет Windows 10 обновления качества.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ecfddf24b8e2550f55c28ef60e218b5caae985da
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861600"
---
# <a name="qualityupdatereference-resource-type"></a>тип ресурса qualityUpdateReference

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Windows 10 обновления качества.

В развертывании такая же ссылка на обновление качества может привести к тому, что устройства получают различные изменения обновления, но контент считается контекстуальным эквивалентом для всех устройств в развертывании.

Наследует [от windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md). Базовый [тип ускоренногоQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|classification|microsoft.graph.windowsUpdates.qualityUpdateClassification|Указывает классификацию указанного контента. Поддерживает подмножество значений **для qualityUpdateClassification.** Возможные значения: `security`, `unknownFutureValue`.|
|releaseDateTime|DateTimeOffset|Указывает обновление качества в указанной службеChannel с указанной классификацией по дате (например, последнее обновление, опубликованное в указанную дату). Значение по умолчанию — `security`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)"
}
```

