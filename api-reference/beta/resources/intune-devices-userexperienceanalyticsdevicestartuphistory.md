---
title: Тип ресурса userExperienceAnalyticsDeviceStartupHistory
description: Сущность истории запуска устройства аналитики пользовательского интерфейса содержит сведения о производительности загрузки устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3cb90d128b32a4bba2038beccd06c0d439f5a97f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159565"
---
# <a name="userexperienceanalyticsdevicestartuphistory-resource-type"></a>Тип ресурса userExperienceAnalyticsDeviceStartupHistory

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность истории запуска устройства аналитики пользовательского интерфейса содержит сведения о производительности загрузки устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsDeviceStartupHistories](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-list.md)|[Коллекция userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Список свойств и связей [объектов userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Get userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Чтение свойств и связей объекта [userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Создание userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-create.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Создание объекта [userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Удаление userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Обновление userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор истории запуска устройства аналитики пользовательского интерфейса.|
|deviceId|String|ИД устройства аналитики пользовательского интерфейса.|
|startTime|DateTimeOffset|Время начала загрузки устройства аналитики пользовательского интерфейса.|
|coreBootTimeInMs|Int32|Время загрузки основного устройства аналитики пользовательского интерфейса в миллисекунах.|
|groupPolicyBootTimeInMs|Int32|Время загрузки групповой политики устройства аналитики пользовательского интерфейса в миллисекунах.|
|featureUpdateBootTimeInMs|Int32|Время обновления функции устройства аналитики пользовательского интерфейса в миллисекунах.|
|totalBootTimeInMs|Int32|Общее время загрузки устройства аналитики пользовательского интерфейса в миллисекунах.|
|groupPolicyLoginTimeInMs|Int32|Время входа в групповую политику устройства аналитики пользовательского интерфейса в миллисекунах.|
|coreLoginTimeInMs|Int32|Время входа в систему устройства аналитики пользовательского интерфейса в миллисекунах.|
|responsiveDesktopTimeInMs|Int32|Аналитика пользовательского интерфейса отвечает за время рабочего стола в миллисекунах.|
|totalLoginTimeInMs|Int32|Общее время входа устройства аналитики пользовательского интерфейса в миллисекунд.|
|isFirstLogin|Boolean|Устройство аналитики пользовательского интерфейса сначала входит в систему.|
|isFeatureUpdate|Boolean|Запись загрузки устройства аналитики пользовательского интерфейса является обновлением функций.|
|operatingSystemVersion|String|Версия операционной системы записи загрузки устройства аналитики пользовательского интерфейса.|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|Категория перезапуска ОС. Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.|
|restartStopCode|String|Код остановки перезапуска ОС. Здесь показан код проверки ошибок, который можно использовать для отслеживания причины синего экрана.|
|restartFaultBucket|String|Сегмент сбоя перезапуска ОС. Сегмент сбоя используется для поиска дополнительных сведений о сбое системы.|

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




