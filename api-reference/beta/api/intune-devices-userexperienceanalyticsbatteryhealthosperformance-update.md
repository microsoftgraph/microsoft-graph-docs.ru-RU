---
title: Обновление userExperienceAnalyticsBatteryHealthOsPerformance
description: Обновление свойств объекта userExperienceAnalyticsBatteryHealthOsPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1798a5a9373d3e924580427627e542a142f10a1e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697476"
---
# <a name="update-userexperienceanalyticsbatteryhealthosperformance"></a>Обновление userExperienceAnalyticsBatteryHealthOsPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthOsPerformance/{userExperienceAnalyticsBatteryHealthOsPerformanceId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)

В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности операционной системы работоспособности батареи для аналитики пользовательского интерфейса.|
|activeDevices|Int32|Количество активных устройств для этой версии ос. Допустимые значения 2147483648 2147483647|
|osVersion|String|Версия операционной системы.|
|osBuildNumber|String|Создайте номер операционной системы.|
|averageMaxCapacityPercentage|Int32|Значение максимальной емкости для всех устройств с определенной версией операционной системы. Максимальная емкость измеряет полную мощность заряда по сравнению с проектной мощностью для аккумуляторов устройства.. Допустимые значения 2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|Значение предполагаемого времени работы на полном заряде для всех устройств с определенной версией операционной системы. Единица в минутах. Допустимые значения 2147483648 2147483647|
|averageBatteryAgeInDays|Int32|Значение времени автономной работы для всех устройств, работающих с определенной версией операционной системы в клиенте. Единица в днях. Допустимые значения 2147483648 2147483647|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthOsPerformance/{userExperienceAnalyticsBatteryHealthOsPerformanceId}
Content-type: application/json
Content-length: 310

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance",
  "activeDevices": 13,
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance",
  "id": "9fc871ad-71ad-9fc8-ad71-c89fad71c89f",
  "activeDevices": 13,
  "osVersion": "Os Version value",
  "osBuildNumber": "Os Build Number value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7
}
```



