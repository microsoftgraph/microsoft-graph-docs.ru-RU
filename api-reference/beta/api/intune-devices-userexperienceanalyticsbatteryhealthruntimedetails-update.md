---
title: Обновление userExperienceAnalyticsBatteryHealthRuntimeDetails
description: Обновление свойств объекта userExperienceAnalyticsBatteryHealthRuntimeDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2a94f510fe550bf7409f2f5e65512fb5bdd19ed
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697492"
---
# <a name="update-userexperienceanalyticsbatteryhealthruntimedetails"></a>Обновление userExperienceAnalyticsBatteryHealthRuntimeDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsBatteryHealthRuntimeDetails.](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)

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
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthRuntimeDetails
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта [userExperienceAnalyticsBatteryHealthRuntimeDetails.](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsBatteryHealthRuntimeDetails.](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта для аналитики пользовательского интерфейса для запуска заряда батареи.|
|activeDevices|Int32|Количество активных устройств в клиенте. Допустимые значения 2147483648 2147483647|
|batteryRuntimeGood|Int32|Количество устройств, время активного запуска которых превышает 5 часов. Допустимые значения 2147483648 2147483647|
|batteryRuntimeFair|Int32|Количество устройств, время активного запуска которых превышает 3 часа, но меньше 5 часов. Допустимые значения 2147483648 2147483647|
|batteryRuntimePoor|Int32|Количество устройств, время активного запуска которых меньше 3 часов. Допустимые значения 2147483648 2147483647|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [userExperienceAnalyticsBatteryHealthRuntimeDetails](../resources/intune-devices-userexperienceanalyticsbatteryhealthruntimedetails.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthRuntimeDetails
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails",
  "activeDevices": 13,
  "batteryRuntimeGood": 2,
  "batteryRuntimeFair": 2,
  "batteryRuntimePoor": 2
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthRuntimeDetails",
  "id": "f6ac1dbf-1dbf-f6ac-bf1d-acf6bf1dacf6",
  "activeDevices": 13,
  "batteryRuntimeGood": 2,
  "batteryRuntimeFair": 2,
  "batteryRuntimePoor": 2
}
```



