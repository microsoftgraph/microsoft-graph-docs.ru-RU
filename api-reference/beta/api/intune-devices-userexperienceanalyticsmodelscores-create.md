---
title: Создание объекта userExperienceAnalyticsModelScores
description: Создайте объект userExperienceAnalyticsModelScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 577f24cb3b6326d532382ef0aaabac4b79304d17
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858375"
---
# <a name="create-userexperienceanalyticsmodelscores"></a>Создание объекта userExperienceAnalyticsModelScores

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте объект [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .

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
POST /deviceManagement/userExperienceAnalyticsModelScores
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта userExperienceAnalyticsModelScores в формате JSON.

В следующей таблице показаны свойства, необходимые при создании объекта userExperienceAnalyticsModelScores.

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
В случае успешного выполнения `201 Created` этот метод возвращает код отклика и объект [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsModelScores
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
HTTP/1.1 201 Created
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




