---
title: тип ресурса userExperienceAnalyticsCategory
description: Объект аналитики пользовательского опыта содержит оценки и сведения о различных метриках категории.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82cc07ff207f74593543c5a1a70c4fe524d92f17
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803772"
---
# <a name="userexperienceanalyticscategory-resource-type"></a>тип ресурса userExperienceAnalyticsCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект аналитики пользовательского опыта содержит оценки и сведения о различных метриках категории.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get userExperienceAnalyticsCategory](../api/intune-devices-userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Чтение свойств и связей [объекта userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)|
|[Обновление userExperienceAnalyticsCategory](../api/intune-devices-userexperienceanalyticscategory-update.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Обновление свойств объекта [userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор категории аналитики пользовательских интерфейсов.|
|overallScore|Int32|Общая оценка категории аналитики пользовательских интерфейсов.|
|totalDevices|Int32|Общее число устройств категории аналитики пользовательских интерфейсов.|
|insights|[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)|Сведения о категории аналитики пользовательских интерфейсов.|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние здоровья категории аналитики пользовательских интерфейсов. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|metricValues|[коллекция userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|Метрические значения для категории аналитики пользовательских интерфейсов.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "overallScore": 1024,
  "totalDevices": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
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
  ],
  "state": "String"
}
```



