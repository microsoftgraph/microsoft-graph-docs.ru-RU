---
title: Создание userExperienceAnalyticsAppHealthDevicePerformance
description: Создание нового объекта userExperienceAnalyticsAppHealthDevicePerformance.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5061d9e34f8646e8c23b3424cb463efde64a8b9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59018301"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformance"></a>Создание userExperienceAnalyticsAppHealthDevicePerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта userExperienceAnalyticsAppHealthDevicePerformance.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsAppHealthDevicePerformance.

В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsAppHealthDevicePerformance.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта производительности устройства для аналитики пользовательского интерфейса.|
|deviceModel|String|Имя модели устройства.|
|deviceManufacturer|Строка|Имя производителя устройства.|
|appCrashCount|Int32|Количество сбоей приложения для устройства. Допустимые значения 2147483648 2147483647|
|crashedAppCount|Int32|Количество различных сбоей приложения для устройства. Допустимые значения 2147483648 2147483647|
|appHangCount|Int32|Для устройства зависает число приложений. Допустимые значения 2147483648 2147483647|
|processedDateTime|DateTimeOffset|Дата и время последнего вычисления статистики.|
|meanTimeToFailureInMinutes|Int32|Время сбоя устройства в минутах. Допустимые значения 2147483648 2147483647|
|deviceAppHealthScore|Двойное с плавающей точкой|Оценка состояния приложения устройства. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|deviceAppHealthStatus|Строка|Общее состояние состояния здоровья приложения на устройстве.|
|deviceId|String|ID устройства.|
|deviceDisplayName|String|Имя устройства.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и `201 Created` [объект userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance
Content-type: application/json
Content-length: 551

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "processedDateTime": "2017-01-01T00:03:22.2339319-08:00",
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
Content-Length: 600

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "2c651499-1499-2c65-9914-652c9914652c",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "processedDateTime": "2017-01-01T00:03:22.2339319-08:00",
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```



