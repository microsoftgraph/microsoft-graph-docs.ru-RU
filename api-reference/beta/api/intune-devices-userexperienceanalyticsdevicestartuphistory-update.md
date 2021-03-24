---
title: Обновление userExperienceAnalyticsDeviceStartupHistory
description: Обновление свойств объекта userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17eccd604ae452bb169fe4d7eb82f97ed1bc51ab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146232"
---
# <a name="update-userexperienceanalyticsdevicestartuphistory"></a>Обновление userExperienceAnalyticsDeviceStartupHistory

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)

В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор истории запуска устройства аналитики пользовательского интерфейса.|
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
|isFirstLogin|Boolean|Устройство аналитики пользовательского интерфейса сначала входит в систему.|
|isFeatureUpdate|Boolean|Запись загрузки устройства для аналитики пользовательского интерфейса — это обновление функций.|
|operatingSystemVersion|String|Версия операционной системы записи операционной системы для аналитики пользовательского интерфейса устройства.|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|Категория перезапуска ОС. Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.|
|restartStopCode|Строка|Код остановки перезапуска ОС. Здесь показан код проверки ошибок, который можно использовать для проверки причины синего экрана.|
|restartFaultBucket|Строка|Ковш перезапуска неисправности ОС. Ведро неисправностей используется для поиска дополнительных сведений о сбое системы.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory/{userExperienceAnalyticsDeviceStartupHistoryId}
Content-type: application/json
Content-length: 680

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 729

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "13357123-7123-1335-2371-351323713513",
  "deviceId": "Device Id value",
  "startTime": "2017-01-01T00:03:29.2730865-08:00",
  "coreBootTimeInMs": 0,
  "groupPolicyBootTimeInMs": 7,
  "featureUpdateBootTimeInMs": 9,
  "totalBootTimeInMs": 1,
  "groupPolicyLoginTimeInMs": 8,
  "coreLoginTimeInMs": 1,
  "responsiveDesktopTimeInMs": 9,
  "totalLoginTimeInMs": 2,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "Operating System Version value",
  "restartCategory": "restartWithUpdate",
  "restartStopCode": "Restart Stop Code value",
  "restartFaultBucket": "Restart Fault Bucket value"
}
```




