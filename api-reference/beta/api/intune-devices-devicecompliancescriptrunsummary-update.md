---
title: Обновление deviceComplianceScriptRunSummary
description: Обновление свойств объекта deviceComplianceScriptRunSummary.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99770521bf349732fbf8fe3b6b35333fa6abb53e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108151"
---
# <a name="update-devicecompliancescriptrunsummary"></a>Обновление deviceComplianceScriptRunSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)

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
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта deviceComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)

В следующей таблице показаны свойства, необходимые при создании [устройстваComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша скрипта соответствия устройству запускать сводную сущность. Это свойство доступно только для чтения.|
|noIssueDetectedDeviceCount|Int32|Количество устройств, для которых сценарий обнаружения не нашел проблемы и устройство является здоровым. Допустимые значения 2147483648 2147483647|
|issueDetectedDeviceCount|Int32|Количество устройств, для которых скрипт обнаружения обнаружил проблему. Допустимые значения 2147483648 2147483647|
|detectionScriptErrorDeviceCount|Int32|Количество устройств, на которых при выполнении скрипта обнаружения произошла ошибка и не была завершена. Допустимые значения 2147483648 2147483647|
|detectionScriptPendingDeviceCount|Int32|Количество устройств, которые еще не запускают последнюю версию сценария соответствия требованиям. Допустимые значения 2147483648 2147483647|
|lastScriptRunDateTime|DateTimeOffset|Время последнего запуска сценария на всех устройствах|



## <a name="response"></a>Отклик
В случае успешного использования этот метод возвращает код ответа и обновленный объект `200 OK` [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "dad42f14-2f14-dad4-142f-d4da142fd4da",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```



