---
title: тип ресурса userExperienceAnalyticsInsight
description: Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 091ac9a6513dc97c80560009b219a5c57d3da14a2808fac1477607f98d5aae47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213125"
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




