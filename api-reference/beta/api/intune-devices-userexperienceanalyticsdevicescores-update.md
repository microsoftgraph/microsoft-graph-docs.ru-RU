---
title: Обновление объектов userExperienceAnalyticsDeviceScores
description: Обновление свойств объекта userExperienceAnalyticsDeviceScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5475a5db4b0ea69b04d99c6fe6e91fdb7424027b
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857990"
---
# <a name="update-userexperienceanalyticsdevicescores"></a>Обновление объектов userExperienceAnalyticsDeviceScores

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [userExperienceAnalyticsDeviceScores в формате](../resources/intune-devices-userexperienceanalyticsdevicescores.md) JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства оценки устройства аналитики пользовательского интерфейса.|
|deviceName|String|Имя устройства аналитики пользовательского интерфейса.|
|model|String|Модель устройства аналитики пользовательского интерфейса.|
|manufacturer|String|Производитель устройства аналитики пользовательского интерфейса.|
|endpointAnalyticsScore|Двойное с плавающей точкой|Оценка устройства аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|startupPerformanceScore|Двойное с плавающей точкой|Оценка производительности при запуске устройства аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|appReliabilityScore|Двойное с плавающей точкой|Оценка надежности приложения для аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|workFromAnywhereScore|Двойное с плавающей точкой|Устройство аналитики пользовательского интерфейса работает отовсюду. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|batteryHealthScore|Двойное с плавающей точкой|Оценка работоспособности батареи устройства аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние работоспособности устройства аналитики пользовательского интерфейса. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае успешного выполнения `200 OK` этот метод возвращает код отклика и обновленный объект [userExperienceAnalyticsDeviceScores](../resources/intune-devices-userexperienceanalyticsdevicescores.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScores/{userExperienceAnalyticsDeviceScoresId}
Content-type: application/json
Content-length: 427

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "workFromAnywhereScore": 7.0,
  "batteryHealthScore": 6.0,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceScores",
  "id": "0dd9f6cf-f6cf-0dd9-cff6-d90dcff6d90d",
  "deviceName": "Device Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "workFromAnywhereScore": 7.0,
  "batteryHealthScore": 6.0,
  "healthStatus": "insufficientData"
}
```




