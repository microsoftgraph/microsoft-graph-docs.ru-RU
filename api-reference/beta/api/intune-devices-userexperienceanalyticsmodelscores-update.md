---
title: Обновление userExperienceAnalyticsModelScores
description: Обновление свойств объекта userExperienceAnalyticsModelScores.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5bfa942664e3ea9690e0c53bc962ef12df6b7a7d
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291908"
---
# <a name="update-userexperienceanalyticsmodelscores"></a>Обновление userExperienceAnalyticsModelScores

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .

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
PATCH /deviceManagement/userExperienceAnalyticsModelScores/{userExperienceAnalyticsModelScoresId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) .

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор модели аналитики пользовательского интерфейса засмеяет объект.|
|model|String|Уникальный идентификатор оценки моделей аналитики пользовательских интерфейсов: модель устройства.|
|manufacturer|String|Уникальный идентификатор оценки моделей аналитики пользовательских интерфейсов: производитель устройств.|
|modelDeviceCount|Int64|Количество устройств модели аналитики пользовательских интерфейсов. Допустимые значения -9.2237203685478E+18 до 9.22337203685478E+18|
|endpointAnalyticsScore|Double|Оценка модели аналитики пользовательского опыта. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|startupPerformanceScore|Double|Оценка производительности запуска модели аналитики пользовательских интерфейсов. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|appReliabilityScore|Double|Оценка надежности приложения для аналитики пользовательского интерфейса. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|workFromAnywhereScore|Double|Модель аналитики пользовательских интерфейсов работает из любой точки. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние состояния модели аналитики пользовательских интерфейсов. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае успеха этот метод `200 OK` возвращает код отклика и обновленный [объект userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsModelScores/{userExperienceAnalyticsModelScoresId}
Content-type: application/json
Content-length: 384

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
  "endpointAnalyticsScore": 7.333333333333333,
  "startupPerformanceScore": 7.666666666666667,
  "appReliabilityScore": 6.333333333333333,
  "workFromAnywhereScore": 7.0,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

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
  "healthStatus": "insufficientData"
}
```




