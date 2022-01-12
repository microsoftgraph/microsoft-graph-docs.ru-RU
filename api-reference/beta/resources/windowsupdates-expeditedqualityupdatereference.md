---
title: ускоренный тип ресурсаQualityUpdateReference
description: Представляет Windows 10 обновления качества для ускорения.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: fa89e4c7cb8a20431b07b88e4d2eb92193d7148c
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61861160"
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

