---
title: тип ресурса userExperienceAnalyticsInsight
description: Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d0d5baaded847858ef91725ff52d8cc1e1d8e02
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794401"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a>тип ресурса userExperienceAnalyticsInsight

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userExperienceAnalyticsMetricId|Строка|Уникальный идентификатор аналитики пользовательского интерфейса.|
|insightId|Строка|Уникальный идентификатор аналитики пользовательского интерфейса.|
|values|[коллекция userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)|Значение аналитики пользовательского интерфейса.|
|severity|[userExperienceAnalyticsInsightSeverity](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|Значение аналитики пользовательского интерфейса. Возможные значения: `none`, `informational`, `warning`, `error`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "userExperienceAnalyticsMetricId": "String",
  "insightId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble",
      "value": "4.2"
    }
  ],
  "severity": "String"
}
```



