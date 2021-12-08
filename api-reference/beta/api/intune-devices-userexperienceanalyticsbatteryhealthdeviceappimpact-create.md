---
title: Создание userExperienceAnalyticsBatteryHealthDeviceAppImpact
description: Создание нового объекта userExperienceAnalyticsBatteryHealthDeviceAppImpact.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93768dc28a2c2f2991d70b9b59f809c6e0ad086e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342701"
---
# <a name="create-userexperienceanalyticsbatteryhealthdeviceappimpact"></a>Создание userExperienceAnalyticsBatteryHealthDeviceAppImpact

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsBatteryHealthDeviceAppImpact.](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBatteryHealthDeviceAppImpact
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsBatteryHealthDeviceAppImpact.

В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsBatteryHealthDeviceAppImpact.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта приложения-приложения для аналитики пользовательского интерфейса.|
|deviceId|String|Уникальный идентификатор устройства, идентификатор устройства Intune DeviceID или SCCM.|
|appName|String|Имя приложения. Например: oltk.exe|
|appDisplayName|String|Удобное для пользователя имя отображения приложения. Например: Outlook|
|appPublisher|String|Издатель приложения. Например: корпорация Майкрософт|
|isForegroundApp|Boolean|верно, если у пользователя было активное взаимодействие с приложением.|
|batteryUsagePercentage|Double|Процент общей мощности батареи, используемой этим приложением, когда устройство не подключено к заряду переменного тока, составляет более 14 дней. Единица в процентах. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsBatteryHealthDeviceAppImpact](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceappimpact.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthDeviceAppImpact
Content-type: application/json
Content-length: 324

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact",
  "deviceId": "Device Id value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "isForegroundApp": true,
  "batteryUsagePercentage": 7.333333333333333
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 373

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDeviceAppImpact",
  "id": "30a55e18-5e18-30a5-185e-a530185ea530",
  "deviceId": "Device Id value",
  "appName": "App Name value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "isForegroundApp": true,
  "batteryUsagePercentage": 7.333333333333333
}
```




