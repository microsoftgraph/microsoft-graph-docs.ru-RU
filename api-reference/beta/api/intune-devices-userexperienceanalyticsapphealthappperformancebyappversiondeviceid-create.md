---
title: Создание userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
description: Создайте новый объект userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf3fc86212cc0c00f7152fee82ccc67912f2fe46
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259384"
---
# <a name="create-userexperienceanalyticsapphealthappperformancebyappversiondeviceid"></a>Создание userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDeviceId
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.

В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности приложения для аналитики пользовательского интерфейса.|
|deviceId|String|ID устройства.|
|deviceDisplayName|String|Имя устройства.|
|processedDateTime|DateTimeOffset|Дата и время последнего вычисления статистики.|
|appName|String|Имя приложения.|
|appDisplayName|String|Удобное имя приложения.|
|appPublisher|Строка|Издатель приложения.|
|appVersion|Строка|Версия приложения.|
|appCrashCount|Int32|Количество сбоей для приложения. Допустимые значения 2147483648 2147483647|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и `201 Created` [объект userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDeviceId
Content-type: application/json
Content-length: 439

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "processedDateTime": "2017-01-01T00:03:22.2339319-08:00",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "appCrashCount": 13
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 488

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId",
  "id": "2dad85e9-85e9-2dad-e985-ad2de985ad2d",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "processedDateTime": "2017-01-01T00:03:22.2339319-08:00",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "appCrashCount": 13
}
```




