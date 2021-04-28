---
title: ускоренный тип ресурсаQualityUpdateReference
description: Представляет Windows 10 обновления качества для ускорения.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 685f65d8c5661cd4c8308ed712ab3fddedbae51d
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068176"
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
|classification|microsoft.graph.windowsUpdates.qualityUpdateClassification|Указывает классификацию указанного контента. Поддерживает подмножество значений **для qualityUpdateClassification.** Значение по умолчанию — `security`. Возможные значения: `security` . Наследуется [от qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).|
|equivalentContent|microsoft.graph.windowsUpdates.equivalentContentOption|Указывает другое содержимое, которое следует считать эквивалентным. Поддерживает подмножество значений **для equivalentContentOption**. Значение по умолчанию — `latestSecurity`. Возможные значения: `latestSecurity` .|
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

