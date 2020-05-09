---
title: Тип ресурса Усерекспериенцеаналитикскатегори
description: Сущность категории аналитики взаимодействия с пользователем содержит показатели и аналитические сведения о различных метриках категории.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d80a287b736786a14eac1244b3e42e07b8e6dad
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178103"
---
# <a name="userexperienceanalyticscategory-resource-type"></a>Тип ресурса Усерекспериенцеаналитикскатегори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность категории аналитики взаимодействия с пользователем содержит показатели и аналитические сведения о различных метриках категории.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Усерекспериенцеаналитикскатегори](../api/intune-devices-userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Чтение свойств и связей объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .|
|[Обновление Усерекспериенцеаналитикскатегори](../api/intune-devices-userexperienceanalyticscategory-update.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|Обновление свойств объекта [усерекспериенцеаналитикскатегори](../resources/intune-devices-userexperienceanalyticscategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор категории аналитики взаимодействия с пользователем.|
|овераллскоре|Int32|Общий показатель категории аналитики взаимодействия с пользователем.|
|insights|Коллекция [усерекспериенцеаналитиксинсигхт](../resources/intune-devices-userexperienceanalyticsinsight.md)|Аналитика для категории аналитики взаимодействия с пользователем.|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Текущее состояние работоспособности категории аналитики взаимодействия с пользователем. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|метриквалуес|Коллекция [усерекспериенцеаналитиксметрик](../resources/intune-devices-userexperienceanalyticsmetric.md)|Значения метрик для категории аналитики взаимодействия с пользователем.|

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



