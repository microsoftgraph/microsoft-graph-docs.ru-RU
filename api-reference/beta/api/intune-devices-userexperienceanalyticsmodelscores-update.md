---
title: Обновление объектов userExperienceAnalyticsModelScores
description: Обновление свойств объекта userExperienceAnalyticsModelScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7964a0ea56aeffb5f166cf3076d9a09aa39092ed
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857878"
---
# <a name="update-userexperienceanalyticsmodelscores"></a>Обновление объектов userExperienceAnalyticsModelScores

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .

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
PATCH /deviceManagement/userExperienceAnalyticsModelScores/{userExperienceAnalyticsModelScoresId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [userExperienceAnalyticsModelScores в формате](../resources/intune-devices-userexperienceanalyticsmodelscores.md) JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта оценки модели аналитики пользовательского интерфейса.|
|model|String|Уникальный идентификатор оценок модели аналитики пользовательского интерфейса: модель устройства.|
|manufacturer|String|Уникальный идентификатор оценок модели аналитики пользовательского интерфейса: производитель устройства.|
|modelDeviceCount|Int64|Число устройств модели аналитики пользовательского интерфейса. Допустимые значения : от -9,22337203685478E+18 до 9,22337203685478E+18|
|endpointAnalyticsScore|Двойное с плавающей точкой|Оценка модели аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|startupPerformanceScore|Двойное с плавающей точкой|Оценка производительности при запуске модели аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|appReliabilityScore|Двойное с плавающей точкой|Оценка надежности приложения модели аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|workFromAnywhereScore|Двойное с плавающей точкой|Модель аналитики пользовательского интерфейса работает отовсюду. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|batteryHealthScore|Двойное с плавающей точкой|Оценка работоспособности батареи модели аналитики пользовательского интерфейса. Допустимые значения — от -1,79769313486232E+308 до 1,79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние работоспособности модели аналитики пользовательского интерфейса. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае успешного выполнения `200 OK` этот метод возвращает код отклика и обновленный объект [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsModelScores/{userExperienceAnalyticsModelScoresId}
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
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
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "id": "f2c0f69c-f69c-f2c0-9cf6-c0f29cf6c0f2",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "workFromAnywhereScore": 7.0,
  "batteryHealthScore": 6.0,
  "healthStatus": "insufficientData"
}
```




