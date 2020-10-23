---
title: Создание Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс
description: Создание нового объекта Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b84784636ff3fe6d4efe5f4644e929c06dfe82f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693180"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformancedetails"></a>Создание Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности устройства аналитики взаимодействия с пользователем.|
|eventDateTime|DateTimeOffset|Время возникновения события.|
|eventType|Строка|Тип события.|
|appDisplayName|String|Понятное имя приложения, для которого произошло событие.|
|deviceId|String|Идентификатор устройства.|
|deviceDisplayName|String|Имя устройства.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерекспериенцеаналитиксапфеалсдевицеперформанцедетаилс](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```





