---
title: тип ресурса userExperienceAnalyticsOverview
description: Объект аналитики пользовательских интерфейсов содержит общую оценку, оценки и сведения по каждой метрике всех категорий.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32466ea9fa14efe0c46b812ac1f6babc9ba32102
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866554"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a>тип ресурса userExperienceAnalyticsOverview

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект аналитики пользовательских интерфейсов содержит общую оценку, оценки и сведения по каждой метрике всех категорий.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Чтение свойств и связей [объекта userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)|
|[Обновление userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Обновление свойств объекта [userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор обзора аналитики пользовательских интерфейсов.|
|overallScore|Int32|Общая оценка аналитики пользовательского опыта.|
|deviceBootPerformanceOverallScore|Int32|Общая оценка производительности загрузки устройства для аналитики пользовательского интерфейса.|
|bestPracticesOverallScore|Int32|Анализ пользовательских интерфейсов позволяет опытом работы с общим показателем.|
|workFromAnywhereOverallScore|Int32|Аналитика пользовательского интерфейса Работает с любого общего балла.|
|appHealthOverallScore|Int32|Общее состояние здоровья приложения для аналитики пользовательского интерфейса.|
|resourcePerformanceOverallScore|Int32|Общая оценка производительности ресурсов аналитики пользовательских ресурсов.|
|insights|[коллекция userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)|Аналитические сведения о пользовательском опыте.|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние состояния состояния аналитики пользовательских интерфейсов. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|deviceBootPerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние состояния состояния аналитики пользовательского интерфейса категории BootPerformance. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|bestPracticesHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices". Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|workFromAnywhereHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние состояния здоровья аналитики пользовательских интерфейсов категории WorkFromAnywhere. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|appHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние здоровья категории аналитики пользовательских интерфейсов "BestPractices". Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|resourcePerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние состояния здоровья в категории аналитики пользовательского интерфейса "ResourcePerformance". Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": 1024,
  "deviceBootPerformanceOverallScore": 1024,
  "bestPracticesOverallScore": 1024,
  "workFromAnywhereOverallScore": 1024,
  "appHealthOverallScore": 1024,
  "resourcePerformanceOverallScore": 1024,
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
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String",
  "workFromAnywhereHealthState": "String",
  "appHealthState": "String",
  "resourcePerformanceHealthState": "String"
}
```




