---
title: Тип ресурса Усерекспериенцеаналитиксдевицеперформанце
description: Объект производительности устройства аналитики взаимодействия с пользователем содержит сведения о быстродействии при загрузке устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df483f340be87ea4c19f4ae2457b678992eb1c94
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684794"
---
# <a name="userexperienceanalyticsdeviceperformance-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксдевицеперформанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект производительности устройства аналитики взаимодействия с пользователем содержит сведения о быстродействии при загрузке устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксдевицеперформанцес](../api/intune-devices-userexperienceanalyticsdeviceperformance-list.md)|Коллекция [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Список свойств и связей объектов [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Получение Усерекспериенцеаналитиксдевицеперформанце](../api/intune-devices-userexperienceanalyticsdeviceperformance-get.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Создание Усерекспериенцеаналитиксдевицеперформанце](../api/intune-devices-userexperienceanalyticsdeviceperformance-create.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Создание нового объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Удаление Усерекспериенцеаналитиксдевицеперформанце](../api/intune-devices-userexperienceanalyticsdeviceperformance-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).|
|[Обновление Усерекспериенцеаналитиксдевицеперформанце](../api/intune-devices-userexperienceanalyticsdeviceperformance-update.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Обновление свойств объекта [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Функция Суммаризедевицеперформанцедевицес](../api/intune-devices-userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices.md)|Коллекция [усерекспериенцеаналитиксдевицеперформанце](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор устройства для загрузки устройства аналитики взаимодействия с пользователем.|
|deviceName|String|Имя устройства службы аналитики взаимодействия с пользователем.|
|model|String|Модель устройства аналитики взаимодействия с пользователем.|
|manufacturer|String|Производитель устройства аналитики взаимодействия с пользователем.|
|diskType|[diskType](../resources/intune-devices-disktype.md)|Тип диска устройства анализа взаимодействия с пользователем. Возможные значения: `unkown`, `hdd`, `ssd`.|
|operatingSystemVersion|String|Версия операционной системы устройства аналитики взаимодействия с пользователем.|
|бутскоре|Int32|Оценка загрузки устройства Analytics User Experience.|
|коребуттимеинмс|Int32|Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).|
|граупполицибуттимеинмс|Int32|Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).|
|хеалсстатус|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние работоспособности устройства аналитики взаимодействия с пользователем. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|логинскоре|Int32|Оценка имени для входа на устройство аналитики взаимодействия с пользователем.|
|корелогинтимеинмс|Int32|Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).|
|граупполицилогинтимеинмс|Int32|Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).|
|deviceCount|Int64|Число устройств для аналитики взаимодействия с пользователем.|
|респонсиведесктоптимеинмс|Int32|Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.|
|блуескринкаунт|Int32|Число синих экранов за последние 14 дней. Допустимые значения — от 0 до 9999999|
|restartCount|Int32|Количество перезапусков за последние 14 дней. Допустимые значения — от 0 до 9999999|
|аверажеблуескринс|Двойное с плавающей точкой|Среднее (среднее) количество синих экранов на устройство за последние 14 дней. Допустимые значения — от 0 до 9999999|
|аверажерестартс|Двойное с плавающей точкой|Средняя (среднее) Количество перезапусков на устройство за последние 14 дней. Допустимые значения — от 0 до 9999999|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "String (identifier)",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "diskType": "String",
  "operatingSystemVersion": "String",
  "bootScore": 1024,
  "coreBootTimeInMs": 1024,
  "groupPolicyBootTimeInMs": 1024,
  "healthStatus": "String",
  "loginScore": 1024,
  "coreLoginTimeInMs": 1024,
  "groupPolicyLoginTimeInMs": 1024,
  "deviceCount": 1024,
  "responsiveDesktopTimeInMs": 1024,
  "blueScreenCount": 1024,
  "restartCount": 1024,
  "averageBlueScreens": "4.2",
  "averageRestarts": "4.2"
}
```





