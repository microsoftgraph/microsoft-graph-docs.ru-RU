---
title: Тип ресурса topicModelingSettings
description: Представляет параметры моделирования тем для дела обнаружения электронных данных
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a021febfda5cd37845f8423de60e0a5a5782325e
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839638"
---
# <a name="topicmodelingsettings-resource-type"></a>Тип ресурса topicModelingSettings

Пространство имен: microsoft.graph.security



Представляет параметры моделирования тем для дела обнаружения электронных данных. Дополнительные сведения см. в разделе "Настройка параметров поиска и аналитики[" в службе обнаружения электронных данных (цен. категория "Премиум").](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|dynamicallyAdjustTopicCount|Логический|Указывает, должна ли модель тем динамически оптимизировать количество созданных разделов. Дополнительные сведения см. в статье ["Динамическое изменение максимального числа тем"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|
|ignoreNumbers|Логический|Указывает, должна ли модель тем исключать числа при анализе текста документа. Дополнительные сведения см. в [статье "Включение чисел в темы"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|
|isEnabled|Boolean|Указывает, включена ли модель тем для дела.|
|topicCount|Int32|Общее количество разделов, которые модель тем создаст для набора для проверки. Дополнительные сведения см. в [разделе "Максимальное количество тем"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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

