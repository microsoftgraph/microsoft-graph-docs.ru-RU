---
title: Тип ресурса userExperienceAnalyticsDeviceScores
description: Сущность оценки устройств аналитики пользовательского интерфейса объединяет различные оценки аналитики конечных точек.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c522277aac0e9122bc597b470102aa2f2aaf4254
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858137"
---
# <a name="userexperienceanalyticsdevicescores-resource-type"></a>Тип ресурса userExperienceAnalyticsDeviceScores

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность оценки устройств аналитики пользовательского интерфейса объединяет различные оценки аналитики конечных точек.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-list.md)|[Коллекция userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Список свойств и связей объектов [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .|
|[Получение userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-get.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Чтение свойств и связей объекта [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .|
|[Создание объекта userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-create.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Создайте объект [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .|
|[Удаление userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-delete.md)|Нет|Удаляет [объект userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md).|
|[Обновление объектов userExperienceAnalyticsDeviceScores](../api/intune-devices-userexperienceanalyticsdevicescores-update.md)|[userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор устройства оценки устройства аналитики пользовательского интерфейса.|
|deviceName|String|Имя устройства аналитики пользовательского интерфейса.|
|model|String|Модель устройства аналитики пользовательского интерфейса.|
|manufacturer|String|Производитель устройства аналитики пользовательского интерфейса.|
|endpointAnalyticsScore|Двойное с плавающей точкой|Оценка устройства аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|startupPerformanceScore|Двойное с плавающей точкой|Оценка производительности при запуске устройства аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|appReliabilityScore|Двойное с плавающей точкой|Оценка надежности приложения для аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|workFromAnywhereScore|Двойное с плавающей точкой|Устройство аналитики пользовательского интерфейса работает отовсюду. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|batteryHealthScore|Двойное с плавающей точкой|Оценка работоспособности батареи устройства аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние работоспособности устройства аналитики пользовательского интерфейса. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceScores"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "String (identifier)",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "endpointAnalyticsScore": "4.2",
  "startupPerformanceScore": "4.2",
  "appReliabilityScore": "4.2",
  "workFromAnywhereScore": "4.2",
  "batteryHealthScore": "4.2",
  "healthStatus": "String"
}
```




