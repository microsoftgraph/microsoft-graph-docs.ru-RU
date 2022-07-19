---
title: Тип ресурса redundancyDetectionSettings
description: Представляет параметры избыточности для дела обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 3717992dc8cc9d1be843430c0a517f081e9bf220
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837529"
---
# <a name="redundancydetectionsettings-resource-type"></a>Тип ресурса redundancyDetectionSettings

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры избыточности (цепочки электронной почты и почти повторяющееся обнаружение) для дела обнаружения электронных данных.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включена ли потоковая обработка электронной почты и обнаружение практически повторяющихся сообщений.|
|maxWords|Int32|Указывает максимальное число слов, используемых для потоков электронной почты и обнаружения практически дубликатов. Дополнительные сведения см. в разделе ["Минимальное или максимальное число слов"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|
|minWords|Int32|Указывает минимальное количество слов, используемых для потоков электронной почты и обнаружения практически повторяющихся сообщений. Дополнительные сведения см. в разделе ["Минимальное или максимальное число слов"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|
|similarityThreshold|Int32|Задает уровень подобия для документов, помещаемого в один и тот же почти повторяющийся набор. Дополнительные сведения см. в статье о пороговом значении сходства документов [и сообщений электронной почты](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.redundancyDetectionSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```

