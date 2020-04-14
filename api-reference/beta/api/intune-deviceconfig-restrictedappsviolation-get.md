---
title: Получение Рестриктедаппсвиолатион
description: Чтение свойств и связей объекта Рестриктедаппсвиолатион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bded226cf7e86558ec7626847c0ec27f06b8156e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431716"
---
# <a name="get-restrictedappsviolation"></a>Получение Рестриктедаппсвиолатион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 664

{
  "value": {
    "@odata.type": "#microsoft.graph.restrictedAppsViolation",
    "id": "53f99903-9903-53f9-0399-f9530399f953",
    "userId": "User Id value",
    "userName": "User Name value",
    "managedDeviceId": "Managed Device Id value",
    "deviceName": "Device Name value",
    "deviceConfigurationId": "Device Configuration Id value",
    "deviceConfigurationName": "Device Configuration Name value",
    "platformType": "androidForWork",
    "restrictedAppsState": "notApprovedApps",
    "restrictedApps": [
      {
        "@odata.type": "microsoft.graph.managedDeviceReportedApp",
        "appId": "App Id value"
      }
    ]
  }
}
```



