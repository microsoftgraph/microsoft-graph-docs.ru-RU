---
title: Обновление userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId
description: Обновление свойств объекта userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 899c3b3adbeacaea58ac1e2035e383d3cacd41cf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59070589"
---
# <a name="update-userexperienceanalyticsapphealthappperformancebyappversiondeviceid"></a>Обновление userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDeviceId/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceIdId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)

В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId.](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md)

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
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceId](../resources/intune-devices-userexperienceanalyticsapphealthappperformancebyappversiondeviceid.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformanceByAppVersionDeviceId/{userExperienceAnalyticsAppHealthAppPerformanceByAppVersionDeviceIdId}
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
HTTP/1.1 200 OK
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



