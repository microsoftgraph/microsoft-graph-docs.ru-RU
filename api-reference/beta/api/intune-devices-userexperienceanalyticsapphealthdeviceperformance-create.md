---
title: Создание Усерекспериенцеаналитиксапфеалсдевицеперформанце
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсдевицеперформанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef02600ac660ab328e79df1da68be17c4f1776ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202852"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformance"></a>Создание Усерекспериенцеаналитиксапфеалсдевицеперформанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсдевицеперформанце в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсдевицеперформанце.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности устройства аналитики взаимодействия с пользователем.|
|deviceModel|String|Имя модели устройства.|
|девицемануфактурер|String|Название изготовителя устройства.|
|аппкрашкаунт|Int32|Количество сбоев приложений для устройства. Допустимые значения: от 2147483648 до 2147483647|
|крашедаппкаунт|Int32|Количество отдельных сбоев приложений для устройства. Допустимые значения: от 2147483648 до 2147483647|
|апфангкаунт|Int32|Количество зависаний приложения для устройства. Допустимые значения: от 2147483648 до 2147483647|
|меантиметофаилуреинминутес|Int32|Среднее время до сбоя устройства в минутах. Допустимые значения: от 2147483648 до 2147483647|
|девицеапфеалсскоре|Двойное с плавающей точкой|Показатель работоспособности приложения для устройства. Допустимые значения — 1 79769313486232e308 E + 308 — 1 79769313486232e308 E + 308|
|девицеапфеалсстатус|String|Общее состояние работоспособности приложений для устройства.|
|deviceId|String|Идентификатор устройства.|
|deviceDisplayName|String|Имя устройства.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсдевицеперформанце](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "2c651499-1499-2c65-9914-652c9914652c",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




