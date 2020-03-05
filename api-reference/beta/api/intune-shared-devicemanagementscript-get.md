---
title: Получение deviceManagementScript
description: Чтение свойств и связей объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3eb1b960b0153ca3201b816863b3de2a7ed8d96d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458492"
---
# <a name="get-devicemanagementscript"></a>Получение deviceManagementScript

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
| &nbsp;&nbsp; **Набор политик** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений||
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
| &nbsp;&nbsp; **Набор политик** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
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
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScript",
    "id": "59ea4525-4525-59ea-2545-ea592545ea59",
    "displayName": "Display Name value",
    "description": "Description value",
    "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
    },
    "scriptContent": "c2NyaXB0Q29udGVudA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "enforceSignatureCheck": true,
    "fileName": "File Name value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "runAs32Bit": true
  }
}
```








