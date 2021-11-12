---
title: тип ресурса qualityUpdateReference
description: Представляет Windows 10 обновления качества.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: bae1315caf6efd2096f9039ca774db18f0b6b764
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890761"
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

