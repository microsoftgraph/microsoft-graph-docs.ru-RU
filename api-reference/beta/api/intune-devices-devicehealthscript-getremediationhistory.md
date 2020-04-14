---
title: Функция Жетремедиатионхистори
description: Функция для получения числа исправлений с помощью сценариев работоспособности устройств
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7d071f91e4433edf2eda7d749aaea65a7d686d02
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426466"
---
# <a name="getremediationhistory-function"></a>Функция Жетремедиатионхистори

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Функция для получения числа исправлений с помощью сценариев работоспособности устройств

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
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getRemediationHistory
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успеха эта функция возвращает код `200 OK` отклика и объект [девицехеалсскриптремедиатионхистори](../resources/intune-devices-devicehealthscriptremediationhistory.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/getRemediationHistory
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 420

{
  "value": {
    "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "historyData": [
      {
        "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
        "date": "<Unknown Primitive Type Edm.Date>",
        "remediatedDeviceCount": 5,
        "noIssueDeviceCount": 2
      }
    ]
  }
}
```



