---
title: Обновление userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: Обновление свойств объекта userExperienceAnalyticsAppHealthDevicePerformanceDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9b10b7acc32fa8b5bf510e2771a7738717e5744
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58255411"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformancedetails"></a>Обновление userExperienceAnalyticsAppHealthDevicePerformanceDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)

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
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности устройства для аналитики пользовательского интерфейса.|
|eventDateTime|DateTimeOffset|Время события.|
|eventType|Строка|Тип события.|
|appDisplayName|String|Удобное имя приложения, для которого произошло событие.|
|appPublisher|Строка|Издатель приложения.|
|appVersion|String|Версия приложения.|
|deviceId|String|ID устройства.|
|deviceDisplayName|String|Имя устройства.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




