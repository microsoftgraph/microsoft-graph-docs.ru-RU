---
title: Обновление deviceManagementScriptRunSummary
description: Обновление свойств объекта deviceManagementScriptRunSummary.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d43d79462997d876734274771ee0e33808c04104
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59121846"
---
# <a name="update-devicemanagementscriptrunsummary"></a>Обновление deviceManagementScriptRunSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)

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
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/runSummary
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта deviceManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)

В следующей таблице показаны свойства, необходимые при создании [устройстваManagementScriptRunSummary.](../resources/intune-devices-devicemanagementscriptrunsummary.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша скрипта управления устройствами запустит объект сводки. Это свойство доступно только для чтения.|
|successDeviceCount|Int32|Количество устройств успешности.|
|errorDeviceCount|Int32|Количество устройств ошибки.|
|successUserCount|Int32|Количество пользователей успешности.|
|errorUserCount|Int32|Количество пользователей ошибки.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/runSummary
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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



