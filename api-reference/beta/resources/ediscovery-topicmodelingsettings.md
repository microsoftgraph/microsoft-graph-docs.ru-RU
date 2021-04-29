---
title: тип ресурса topicModelingSettings
description: Параметры моделирования тем для дела об обнаружении электронных данных
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: bd433de0aa88298961366f50425706e1af4bffde
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080878"
---
# <a name="topicmodelingsettings-resource-type"></a>тип ресурса topicModelingSettings

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры моделирования тем (Темы) для дела об обнаружении электронных данных. Дополнительные данные см. в [обзоре Настройка параметров](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)поиска и аналитики в Advanced eDiscovery.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|dynamicallyAdjustTopicCount|Boolean|Дополнительные дополнительные вопросы см. в [см. встраив максимальное количество тем динамически.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)|
|ignoreNumbers|Boolean|Дополнительные данные см. в [дополнительных подробной информации о включаем числа в темы.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)|
|isEnabled|Boolean|Указывает, включены ли темы для дела.|
|topicCount|Int32|Дополнительные дополнительные вопросы см. в дополнительных подробной информации о [максимальном количестве тем.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.topicModelingSettings",
  "isEnabled": "Boolean",
  "ignoreNumbers": "Boolean",
  "topicCount": "Integer",
  "dynamicallyAdjustTopicCount": "Boolean"
}
```
