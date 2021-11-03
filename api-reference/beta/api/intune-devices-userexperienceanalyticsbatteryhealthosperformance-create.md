---
title: Создание userExperienceAnalyticsBatteryHealthOsPerformance
description: Создайте новый объект userExperienceAnalyticsBatteryHealthOsPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8042302c8e79ed0b117a4b6ddf201e7255915dbc
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697479"
---
# <a name="create-userexperienceanalyticsbatteryhealthosperformance"></a>Создание userExperienceAnalyticsBatteryHealthOsPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект userExperienceAnalyticsBatteryHealthOsPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)

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
POST /deviceManagement/userExperienceAnalyticsBatteryHealthOsPerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsBatteryHealthOsPerformance.

В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsBatteryHealthOsPerformance.

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
В случае успеха этот метод возвращает код отклика и объект `201 Created` [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthOsPerformance
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
HTTP/1.1 201 Created
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



