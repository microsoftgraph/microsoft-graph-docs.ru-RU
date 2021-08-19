---
title: тип ресурса userExperienceAnalyticsDeviceStartupHistory
description: Объект истории запуска устройства для аналитики пользовательских интерфейсов содержит сведения об истории производительности загрузки устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d3b435caf5cd8bb3c514eeb602f2397a6e93322754bb4313536ffb33ace5f727
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244717"
---
# <a name="userexperienceanalyticsdevicestartuphistory-resource-type"></a>тип ресурса userExperienceAnalyticsDeviceStartupHistory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект истории запуска устройства для аналитики пользовательских интерфейсов содержит сведения об истории производительности загрузки устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsDeviceStartupHistories](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-list.md)|[коллекция userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Список свойств и связей [объектов userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Get userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Чтение свойств и связей [объекта userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Создание userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-create.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Создание нового [объекта userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Удаление userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).|
|[Обновление userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор истории запуска устройства аналитики пользовательского интерфейса.|
|deviceId|String|ID устройства аналитики пользовательского интерфейса.|
|startTime|DateTimeOffset|Время запуска загрузки устройства для аналитики пользовательского интерфейса.|
|coreBootTimeInMs|Int32|Основное время загрузки устройства для аналитики пользовательского интерфейса в миллисекунд.|
|groupPolicyBootTimeInMs|Int32|Время загрузки групповой политики пользовательского интерфейса устройства в миллисекунд.|
|featureUpdateBootTimeInMs|Int32|Время обновления устройства аналитики пользовательского интерфейса в миллисекундном периоде.|
|totalBootTimeInMs|Int32|Общее время загрузки устройства аналитики пользовательского интерфейса в миллисекунд.|
|groupPolicyLoginTimeInMs|Int32|Время входа в группу политик пользовательского интерфейса для аналитики устройств в миллисекунд.|
|coreLoginTimeInMs|Int32|Время входа основного устройства для аналитики пользовательского интерфейса в миллисекунд.|
|responsiveDesktopTimeInMs|Int32|Аналитика пользовательского интерфейса реагирует на время рабочего стола в миллисекунд.|
|totalLoginTimeInMs|Int32|Общее время входа устройства аналитики пользовательского интерфейса в миллисекунд.|
|isFirstLogin|Логический|Устройство аналитики пользовательского интерфейса сначала входит в систему.|
|isFeatureUpdate|Логический|Запись загрузки устройства для аналитики пользовательского интерфейса — это обновление функций.|
|operatingSystemVersion|String|Версия операционной системы записи операционной системы для аналитики пользовательского интерфейса устройства.|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|Категория перезапуска ОС. Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.|
|restartStopCode|String|Код остановки перезапуска ОС. Здесь показан код проверки ошибок, который можно использовать для проверки причины синего экрана.|
|restartFaultBucket|Строка|Ковш перезапуска неисправности ОС. Ведро неисправностей используется для поиска дополнительных сведений о сбое системы.|

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
  "operatingSystemVersion": "String",
  "restartCategory": "String",
  "restartStopCode": "String",
  "restartFaultBucket": "String"
}
```




