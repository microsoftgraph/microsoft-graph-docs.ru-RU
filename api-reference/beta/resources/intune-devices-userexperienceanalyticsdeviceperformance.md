---
title: тип ресурса userExperienceAnalyticsDevicePerformance
description: Объект пользовательской аналитики производительности устройств содержит сведения о производительности загрузки устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 444168c83f34ad8da35f23b0bee27095e495bc4a
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367680"
---
# <a name="userexperienceanalyticsdeviceperformance-resource-type"></a>тип ресурса userExperienceAnalyticsDevicePerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект пользовательской аналитики производительности устройств содержит сведения о производительности загрузки устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsDevicePerformances](../api/intune-devices-userexperienceanalyticsdeviceperformance-list.md)|[коллекция userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Список свойств и связей [объектов userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Get userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-get.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Чтение свойств и связей [объекта userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Создание userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-create.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Создание нового [объекта userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[Удаление userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md).|
|[Обновление userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-update.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Обновление свойств объекта [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) .|
|[summarizeDevicePerformanceDevices function](../api/intune-devices-userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices.md)|[коллекция userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства загрузки загрузочного устройства для аналитики пользовательского интерфейса.|
|deviceName|String|Имя устройства аналитики пользовательского интерфейса.|
|model|String|Модель устройства аналитики пользовательских интерфейсов.|
|manufacturer|String|Производитель устройств аналитики пользовательских интерфейсов.|
|diskType|[diskType](../resources/intune-devices-disktype.md)|Тип диска для аналитики пользовательского интерфейса устройства. Возможные значения: `unknown`, `hdd`, `ssd`, `unknownFutureValue`.|
|operatingSystemVersion|String|Версия операционной системы для аналитики пользовательского интерфейса устройства.|
|bootScore|Int32|Оценка загрузки устройства для аналитики пользовательского интерфейса.|
|coreBootTimeInMs|Int32|Основное время загрузки устройства для аналитики пользовательского интерфейса в миллисекунд.|
|groupPolicyBootTimeInMs|Int32|Время загрузки групповой политики устройств для пользовательского интерфейса в миллисекунд.|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние здоровья устройства аналитики пользовательского интерфейса. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|loginScore|Int32|Оценка входа устройства аналитики пользовательского интерфейса.|
|coreLoginTimeInMs|Int32|Время входа основного устройства для аналитики пользовательского интерфейса в миллисекунд.|
|groupPolicyLoginTimeInMs|Int32|Время входа в группу политик пользовательского интерфейса для аналитики устройств в миллисекунд.|
|deviceCount|Int64|Аналитика пользовательских интерфейсов суммирует количество устройств.|
|responsiveDesktopTimeInMs|Int32|Аналитика пользовательского интерфейса реагирует на время рабочего стола в миллисекунд.|
|blueScreenCount|Int32|Количество синих экранов за последние 14 дней. Допустимые значения от 0 до 9999999|
|restartCount|Int32|Количество перезапусков за последние 14 дней. Допустимые значения от 0 до 9999999|
|averageBlueScreens|Double|Среднее (среднее) число синих экранов на устройство за последние 14 дней. Допустимые значения от 0 до 9999999|
|averageRestarts|Double|Среднее (среднее) число перезапусков на устройство за последние 14 дней. Допустимые значения от 0 до 9999999|
|startupPerformanceScore|Double|Оценка производительности запуска устройства для аналитики пользовательского интерфейса. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|modelStartupPerformanceScore|Double|Оценка производительности запуска модели аналитики пользовательской модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|

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
  "averageRestarts": "4.2",
  "startupPerformanceScore": "4.2",
  "modelStartupPerformanceScore": "4.2"
}
```




