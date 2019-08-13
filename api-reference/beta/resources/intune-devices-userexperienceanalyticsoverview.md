---
title: Тип ресурса Усерекспериенцеаналитиксовервиев
description: В объекте обзор анализа взаимодействия с пользователем содержатся общие показатели и оценки всех показателей всех категорий.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff3be73059f913943236bfce8bcb4e729a39081d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371546"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксовервиев

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В объекте обзор анализа взаимодействия с пользователем содержатся общие показатели и оценки всех показателей всех категорий.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Усерекспериенцеаналитиксовервиев](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .|
|[Обновление Усерекспериенцеаналитиксовервиев](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md)|Обновление свойств объекта [усерекспериенцеаналитиксовервиев](../resources/intune-devices-userexperienceanalyticsoverview.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для обзора аналитики взаимодействия с пользователем.|
|овераллскоре|Int32|Общий показатель аналитики взаимодействия с пользователем.|
|девицебутперформанцеовераллскоре|Int32|Общая оценка производительности при загрузке устройства Analytics.|
|бестпрактицесовераллскоре|Int32|Общая оценка рекомендаций по анализу пользовательских интерфейсов.|
|insights|Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)|Аналитика взаимодействия с пользователем.|

## <a name="relationships"></a>Отношения
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
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```



