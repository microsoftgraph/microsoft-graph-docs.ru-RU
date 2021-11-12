---
title: ускоренный тип ресурсаQualityUpdateReference
description: Представляет Windows 10 обновления качества для ускорения.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: c3313483305613cf684b066f2ba9569676974b23
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890824"
---
# <a name="expeditedqualityupdatereference-resource-type"></a>ускоренный тип ресурсаQualityUpdateReference

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет Windows 10 обновления качества для ускорения.

В развертывании такая же ссылка на ускоренное обновление качества может привести к тому, что устройства получают различные изменения, но контент считается контекстуальным эквивалентом для всех устройств в развертывании.

Наследует [от qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|classification|microsoft.graph.windowsUpdates.qualityUpdateClassification|Указывает классификацию указанного контента. Поддерживает подмножество значений **для qualityUpdateClassification.** Значение по умолчанию — `security`. Возможные значения: `security`, `unknownFutureValue`. Наследуется [от qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).|
|equivalentContent|microsoft.graph.windowsUpdates.equivalentContentOption|Указывает другое содержимое, которое следует считать эквивалентным. Поддерживает подмножество значений **для equivalentContentOption**. Значение по умолчанию — `latestSecurity`. Возможные значения: `latestSecurity`, `unknownFutureValue`.|
|releaseDateTime|DateTimeOffset|Указывает обновление качества с указанной классификацией **на** дату публикации (то есть последнее обновление, опубликованное в указанную дату). Все устройства с обновлением, которое было опубликовано до **выпускаDateTime,** получат ускоренное обновление качества. Наследуется [от qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)",
  "equivalentContent": "String"
}
```

