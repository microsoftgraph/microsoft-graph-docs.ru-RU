---
title: Обновление deviceManagementScriptRunSummary
description: Обновление свойства объекта deviceManagementScriptRunSummary.
ms.openlocfilehash: 83e45ce7cf01f0fe95b2a4240ebafc1dd88507c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077395"
---
# <a name="update-devicemanagementscriptrunsummary"></a>Обновление deviceManagementScriptRunSummary

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Обновление свойства объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON для объекта [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) .

В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша сценарий управления устройства выполните сводки сущности.|
|successDeviceCount|Int32|Число допустимых устройства.|
|errorDeviceCount|Int32|Число ошибок устройства.|
|successUserCount|Int32|Число пользователей успеха.|
|errorUserCount|Int32|Число пользователей об ошибках.|



## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) объекта в теле ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 108

{
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```





