---
title: Список устройствHealthScripts
description: Список свойств и связей объектов deviceHealthScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 701424d7a87c8c6ebd2926ae5af20f76d2d6882a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146288"
---
# <a name="list-devicehealthscripts"></a>Список устройствHealthScripts

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей [объектов deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1578

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScript",
      "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
      "publisher": "Publisher value",
      "version": "Version value",
      "displayName": "Display Name value",
      "description": "Description value",
      "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
      "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "runAs32Bit": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "isGlobalScript": true,
      "highestAvailableVersion": "Highest Available Version value",
      "detectionScriptParameters": [
        {
          "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
          "name": "Name value",
          "description": "Description value",
          "isRequired": true,
          "applyDefaultValueWhenNotAssigned": true,
          "defaultValue": "Default Value value"
        }
      ],
      "remediationScriptParameters": [
        {
          "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
          "name": "Name value",
          "description": "Description value",
          "isRequired": true,
          "applyDefaultValueWhenNotAssigned": true,
          "defaultValue": "Default Value value"
        }
      ]
    }
  ]
}
```




