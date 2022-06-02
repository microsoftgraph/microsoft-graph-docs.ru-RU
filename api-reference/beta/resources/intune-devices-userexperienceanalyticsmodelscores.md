---
title: Тип ресурса userExperienceAnalyticsModelScores
description: Сущность оценки модели аналитики пользовательского интерфейса объединяет различные оценки аналитики конечных точек.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbf00cd94e9667ac556535b5d8dca75e2a76800a
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857871"
---
# <a name="userexperienceanalyticsmodelscores-resource-type"></a>Тип ресурса userExperienceAnalyticsModelScores

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность оценки модели аналитики пользовательского интерфейса объединяет различные оценки аналитики конечных точек.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-list.md)|[Коллекция userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Список свойств и связей объектов [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Получение объектов userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-get.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Чтение свойств и связей объекта [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Создание объекта userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-create.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Создайте объект [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|
|[Удаление объектов userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-delete.md)|Нет|Удаляет [объект userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md).|
|[Обновление объектов userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-update.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|Обновление свойств объекта [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта оценки модели аналитики пользовательского интерфейса.|
|model|String|Уникальный идентификатор оценок модели аналитики пользовательского интерфейса: модель устройства.|
|manufacturer|String|Уникальный идентификатор оценок модели аналитики пользовательского интерфейса: производитель устройства.|
|modelDeviceCount|Int64|Число устройств модели аналитики пользовательского интерфейса. Допустимые значения : от -9,22337203685478E+18 до 9,22337203685478E+18|
|endpointAnalyticsScore|Двойное с плавающей точкой|Оценка модели аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|startupPerformanceScore|Двойное с плавающей точкой|Оценка производительности при запуске модели аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|appReliabilityScore|Двойное с плавающей точкой|Оценка надежности приложения модели аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|workFromAnywhereScore|Двойное с плавающей точкой|Модель аналитики пользовательского интерфейса работает отовсюду. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|batteryHealthScore|Двойное с плавающей точкой|Оценка работоспособности батареи модели аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние работоспособности модели аналитики пользовательского интерфейса. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Отношения
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
  "batteryHealthScore": "4.2",
  "healthStatus": "String"
}
```




