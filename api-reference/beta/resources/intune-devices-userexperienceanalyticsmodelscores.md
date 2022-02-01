---
title: тип ресурса userExperienceAnalyticsModelScores
description: Модель аналитики пользовательских интерфейсов объединяет различные оценки аналитики конечных точек.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffdcc4697699d3a60b5b52cc3a966ad2c82f1b14
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292006"
---
# <a name="userexperienceanalyticsmodelscores-resource-type"></a>тип ресурса userExperienceAnalyticsModelScores

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Модель аналитики пользовательских интерфейсов объединяет различные оценки аналитики конечных точек.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsModelScoreses](../api/intune-devices-userexperienceanalyticsmodelscores-list.md)|[коллекция userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Список свойств и связей [объектов userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Get userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-get.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Чтение свойств и связей [объекта userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Создание userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-create.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Создание нового [объекта userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Удаление userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md).|
|[Обновление userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-update.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Обновление свойств объекта [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор модели аналитики пользовательского интерфейса засмеяет объект.|
|model|String|Уникальный идентификатор оценки моделей аналитики пользовательских интерфейсов: модель устройства.|
|manufacturer|String|Уникальный идентификатор оценки моделей аналитики пользовательских интерфейсов: производитель устройств.|
|modelDeviceCount|Int64|Количество устройств модели аналитики пользовательских интерфейсов. Допустимые значения -9.2237203685478E+18 до 9.22337203685478E+18|
|endpointAnalyticsScore|Double|Оценка модели аналитики пользовательского опыта. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|startupPerformanceScore|Double|Оценка производительности запуска модели аналитики пользовательских интерфейсов. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|appReliabilityScore|Double|Оценка надежности приложения для аналитики пользовательского интерфейса. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|workFromAnywhereScore|Double|Модель аналитики пользовательских интерфейсов работает из любой точки. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние состояния модели аналитики пользовательских интерфейсов. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsModelScores"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "id": "String (identifier)",
  "model": "String",
  "manufacturer": "String",
  "modelDeviceCount": 1024,
  "endpointAnalyticsScore": "4.2",
  "startupPerformanceScore": "4.2",
  "appReliabilityScore": "4.2",
  "workFromAnywhereScore": "4.2",
  "healthStatus": "String"
}
```




