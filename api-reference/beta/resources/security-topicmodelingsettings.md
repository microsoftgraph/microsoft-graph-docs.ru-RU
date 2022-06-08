---
title: Тип ресурса topicModelingSettings
description: Параметры моделирования тем для дела обнаружения электронных данных
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 865368b2d6d0723a47cc352e64f5400f254b3183
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946056"
---
# <a name="topicmodelingsettings-resource-type"></a>Тип ресурса topicModelingSettings

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры моделирования тем (тем) для дела обнаружения электронных данных. Дополнительные сведения см. в разделе "Настройка параметров поиска и аналитики [" в advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dynamicallyAdjustTopicCount|Boolean|Дополнительные сведения см. в статье ["Динамическое изменение максимального числа тем"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|
|ignoreNumbers|Boolean|Дополнительные сведения см. в [статье "Включение чисел в темы"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|
|isEnabled|Boolean|Указывает, включены ли темы для дела.|
|topicCount|Int32|Дополнительные сведения см. в [разделе "Максимальное количество тем"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.topicModelingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.topicModelingSettings",
  "isEnabled": "Boolean",
  "ignoreNumbers": "Boolean",
  "topicCount": "Integer",
  "dynamicallyAdjustTopicCount": "Boolean"
}
```

