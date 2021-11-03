---
title: Обновление userExperienceAnalyticsBatteryHealthModelPerformance
description: Обновление свойств объекта userExperienceAnalyticsBatteryHealthModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5daf586af1f04c27a66b0bdd12abca85291b04d
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696296"
---
# <a name="update-userexperienceanalyticsbatteryhealthmodelperformance"></a>Обновление userExperienceAnalyticsBatteryHealthModelPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)

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
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthModelPerformance/{userExperienceAnalyticsBatteryHealthModelPerformanceId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)

В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsBatteryHealthModelPerformance.](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности модели работоспособности модели работоспособности пользовательской аналитики.|
|activeDevices|Int32|Количество активных устройств для этой модели. Допустимые значения 2147483648 2147483647|
|model|String|Имя модели устройства.|
|manufacturer|String|Имя производителя устройств.|
|averageMaxCapacityPercentage|Int32|Значение максимальной емкости для всех устройств данной модели. Максимальная емкость измеряет полную мощность заряда по сравнению с проектной мощностью для аккумуляторов устройства.. Допустимые значения 2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|Для всех устройств данной модели имеется в виду предполагаемое время запуска на полную плату. Единица в минутах. Допустимые значения 2147483648 2147483647|
|averageBatteryAgeInDays|Int32|Время работы от батареи для всех устройств данной модели в клиенте. Единица в днях. Допустимые значения 2147483648 2147483647|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthModelPerformance/{userExperienceAnalyticsBatteryHealthModelPerformanceId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "activeDevices": 13,
  "model": "Model value",
  "manufacturer": "Manufacturer value",
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
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "id": "0850afa4-afa4-0850-a4af-5008a4af5008",
  "activeDevices": 13,
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7
}
```



