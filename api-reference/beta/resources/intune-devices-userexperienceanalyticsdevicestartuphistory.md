---
title: Тип ресурса Усерекспериенцеаналитиксдевицестартуфистори
description: Сущность журнала запуска устройства Analytics User Experience содержит подробные сведения о журнале производительности загрузки устройств.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4275053cda78e26093879b64a521870eec21089
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783825"
---
# <a name="userexperienceanalyticsdevicestartuphistory-resource-type"></a>Тип ресурса Усерекспериенцеаналитиксдевицестартуфистори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность журнала запуска устройства Analytics User Experience содержит подробные сведения о журнале производительности загрузки устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерекспериенцеаналитиксдевицестартуфисториес](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-list.md)|Коллекция [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Список свойств и связей объектов [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .|
|[Получение Усерекспериенцеаналитиксдевицестартуфистори](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Чтение свойств и связей объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .|
|[Создание Усерекспериенцеаналитиксдевицестартуфистори](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-create.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Создание нового объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .|
|[Удаление Усерекспериенцеаналитиксдевицестартуфистори](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-delete.md)|Нет|Удаляет объект [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).|
|[Обновление Усерекспериенцеаналитиксдевицестартуфистори](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Обновление свойств объекта [усерекспериенцеаналитиксдевицестартуфистори](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор журнала запуска устройства Analytics User Experience.|
|deviceId|String|Идентификатор устройства службы аналитики взаимодействия с пользователем.|
|startTime|DateTimeOffset|Время начала загрузки устройства Analytics User Experience.|
|коребуттимеинмс|Int32|Время загрузки ядра устройства аналитики для пользователя (в миллисекундах).|
|граупполицибуттимеинмс|Int32|Время загрузки групповой политики устройства Analytics для пользователя (в миллисекундах).|
|феатуреупдатебуттимеинмс|Int32|Время обновления компонента службы аналитики взаимодействия с пользователем (в миллисекундах).|
|тоталбуттимеинмс|Int32|Общее время загрузки устройства Analytics User Experience (в миллисекундах).|
|граупполицилогинтимеинмс|Int32|Время входа в групповую политику устройства Analytics User Experience (в миллисекундах).|
|корелогинтимеинмс|Int32|Время входа в ядро устройства аналитики взаимодействия с пользователем (в миллисекундах).|
|респонсиведесктоптимеинмс|Int32|Время, в течение которого выполняется анализ пользовательского интерфейса на рабочем столе в миллисекундах.|
|тоталлогинтимеинмс|Int32|Общее время входа в систему для устройства аналитики взаимодействия с пользователем (в миллисекундах).|
|исфирстлогин|Логический|Первое имя входа устройства Analytics User Experience.|
|исфеатуреупдате|Логический|Загрузочная запись устройства аналитики взаимодействия с пользователем — это обновление компонентов.|
|operatingSystemVersion|String|Версия операционной системы для записи загрузки устройства службы аналитики взаимодействия с пользователем.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "String (identifier)",
  "deviceId": "String",
  "startTime": "String (timestamp)",
  "coreBootTimeInMs": 1024,
  "groupPolicyBootTimeInMs": 1024,
  "featureUpdateBootTimeInMs": 1024,
  "totalBootTimeInMs": 1024,
  "groupPolicyLoginTimeInMs": 1024,
  "coreLoginTimeInMs": 1024,
  "responsiveDesktopTimeInMs": 1024,
  "totalLoginTimeInMs": 1024,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "String"
}
```



