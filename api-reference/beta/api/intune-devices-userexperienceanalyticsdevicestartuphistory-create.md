---
title: Создание userExperienceAnalyticsDeviceStartupHistory
description: Создание объекта userExperienceAnalyticsDeviceStartupHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2bfbe3272018304da8e959ea9663ccd38119c0fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159677"
---
# <a name="create-userexperienceanalyticsdevicestartuphistory"></a>Создание userExperienceAnalyticsDeviceStartupHistory

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceStartupHistory
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта userExperienceAnalyticsDeviceStartupHistory в JSON.

В следующей таблице показаны свойства, необходимые при создании объекта userExperienceAnalyticsDeviceStartupHistory.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор истории запуска устройства аналитики пользовательского интерфейса.|
|deviceId|String|ИД устройства аналитики пользовательского интерфейса.|
|startTime|DateTimeOffset|Время начала загрузки устройства аналитики пользовательского интерфейса.|
|coreBootTimeInMs|Int32|Время загрузки основного устройства аналитики пользовательского интерфейса в миллисекунах.|
|groupPolicyBootTimeInMs|Int32|Время загрузки групповой политики устройства аналитики пользовательского интерфейса в миллисекунах.|
|featureUpdateBootTimeInMs|Int32|Время обновления функции устройства аналитики пользовательского интерфейса в миллисекунах.|
|totalBootTimeInMs|Int32|Общее время загрузки устройства аналитики пользовательского интерфейса в миллисекунах.|
|groupPolicyLoginTimeInMs|Int32|Время входа в групповую политику устройства аналитики пользовательского интерфейса (в миллисекунах).|
|coreLoginTimeInMs|Int32|Время входа в систему устройства аналитики пользовательского интерфейса в миллисекунах.|
|responsiveDesktopTimeInMs|Int32|Аналитика пользовательского интерфейса отвечает за время рабочего стола в миллисекунах.|
|totalLoginTimeInMs|Int32|Общее время входа устройства аналитики пользовательского интерфейса в миллисекунд.|
|isFirstLogin|Boolean|Устройство аналитики пользовательского интерфейса сначала входит в систему.|
|isFeatureUpdate|Boolean|Запись загрузки устройства аналитики пользовательского интерфейса является обновлением функций.|
|operatingSystemVersion|String|Версия операционной системы записи загрузки устройства аналитики пользовательского интерфейса.|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|Категория перезапуска ОС. Возможные значения: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.|
|restartStopCode|String|Код остановки перезапуска ОС. Здесь показан код проверки ошибок, который можно использовать для отслеживания причины синего экрана.|
|restartFaultBucket|String|Сегмент сбоя перезапуска ОС. Сегмент сбоя используется для поиска дополнительных сведений о сбое системы.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupHistory
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
HTTP/1.1 201 Created
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




