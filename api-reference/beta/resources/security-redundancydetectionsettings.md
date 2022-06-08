---
title: Тип ресурса redundancyDetectionSettings
description: Параметры избыточности для дела обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8fcc425c95540552479cfd07b862e5e9ba29e53e
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946067"
---
# <a name="redundancydetectionsettings-resource-type"></a>Тип ресурса redundancyDetectionSettings

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры избыточности (потоковая обработка электронной почты и обнаружение практически повторяющихся данных) для дела обнаружения электронных данных.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включена ли потоковая обработка электронной почты и обнаружение практически повторяющихся сообщений.|
|maxWords|Int32|Указывает максимальное число слов, используемых для потоков электронной почты и обнаружения практически дубликатов. Дополнительные сведения см. в разделе ["Минимальное или максимальное число слов"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|
|minWords|Int32|Указывает минимальное количество слов, используемых для потоков электронной почты и обнаружения практически повторяющихся сообщений. Дополнительные сведения см. в разделе ["Минимальное или максимальное число слов"](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|
|similarityThreshold|Int32|Задает уровень подобия для документов, помещаемого в один и тот же почти повторяющийся набор. Дополнительные сведения см. в статье о пороговом значении сходства документов [и сообщений электронной почты](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading).|


## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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

