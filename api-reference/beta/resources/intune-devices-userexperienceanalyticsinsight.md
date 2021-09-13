---
title: тип ресурса userExperienceAnalyticsInsight
description: Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e2dfcc6da42943743043674ce17a5619a59bf1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147873"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a>тип ресурса userExperienceAnalyticsInsight

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Анализ пользовательских интерфейсов — это рекомендация по улучшению показателей аналитики пользовательских интерфейсов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userExperienceAnalyticsMetricId|String|Уникальный идентификатор аналитики пользовательского интерфейса.|
|insightId|String|Уникальный идентификатор аналитики пользовательского интерфейса.|
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



