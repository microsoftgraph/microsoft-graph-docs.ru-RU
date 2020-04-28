---
title: Тип ресурса Усерекспериенцеаналитиксовервиев
description: В объекте обзор анализа взаимодействия с пользователем содержатся общие показатели и оценки всех показателей всех категорий.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 56ab161a77f21d06c034322a4daa84c5880db0da
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464988"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксовервиев

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В объекте обзор анализа взаимодействия с пользователем содержатся общие показатели и оценки всех показателей всех категорий.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Усерекспериенцеаналитиксовервиев](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .|
|[Обновление Усерекспериенцеаналитиксовервиев](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|Обновление свойств объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для обзора аналитики взаимодействия с пользователем.|
|овераллскоре|Int32|Общий показатель аналитики взаимодействия с пользователем.|
|девицебутперформанцеовераллскоре|Int32|Общая оценка производительности при загрузке устройства Analytics.|
|бестпрактицесовераллскоре|Int32|Общая оценка рекомендаций по анализу пользовательских интерфейсов.|
|insights|Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)|Аналитика взаимодействия с пользователем.|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние работоспособности в обзоре аналитики взаимодействия с пользователем. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|девицебутперформанцехеалсстате|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние работоспособности категории аналитики взаимодействия с пользователем "Бутперформанце". Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|бестпрактицешеалсстате|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние работоспособности категории аналитики взаимодействия с пользователем "Бестпрактицес". Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

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
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String"
}
```



