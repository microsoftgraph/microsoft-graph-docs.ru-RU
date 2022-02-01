---
title: Обновление userExperienceAnalyticsBatteryHealthCapacityDetails
description: Обновление свойств объекта userExperienceAnalyticsBatteryHealthCapacityDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1407c7ce6f4f76ead2c9004bdaa5c474a040897d
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292055"
---
# <a name="update-userexperienceanalyticsbatteryhealthcapacitydetails"></a>Обновление userExperienceAnalyticsBatteryHealthCapacityDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) .

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
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthCapacityDetails
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта [userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) .

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта емкости аккумулятора для аналитики пользовательского интерфейса.|
|activeDevices|Int32|Количество активных устройств в клиенте. Допустимые значения 2147483648 2147483647|
|batteryCapacityGood|Int32|Количество устройств, максимальная емкость которых превышает 80%. Допустимые значения 2147483648 2147483647|
|batteryCapacityFair|Int32|Количество устройств, максимальная емкость которых превышает 50%, но меньше 80%. Допустимые значения 2147483648 2147483647|
|batteryCapacityPoor|Int32|Количество устройств, максимальная емкость которых составляет менее 50%. Допустимые значения 2147483648 2147483647|
|lastRefreshedDateTime|DateTimeOffset|Записано время даты этого экземпляра сведений о емкости.|



## <a name="response"></a>Отклик
В случае `200 OK` успеха этот метод возвращает код ответа и обновленный объект [userExperienceAnalyticsBatteryHealthCapacityDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthcapacitydetails.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthCapacityDetails
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails",
  "activeDevices": 13,
  "batteryCapacityGood": 3,
  "batteryCapacityFair": 3,
  "batteryCapacityPoor": 3,
  "lastRefreshedDateTime": "2017-01-01T00:02:37.7100903-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthCapacityDetails",
  "id": "b01fc7df-c7df-b01f-dfc7-1fb0dfc71fb0",
  "activeDevices": 13,
  "batteryCapacityGood": 3,
  "batteryCapacityFair": 3,
  "batteryCapacityPoor": 3,
  "lastRefreshedDateTime": "2017-01-01T00:02:37.7100903-08:00"
}
```




