---
title: Список Мобилеапптраублешутинжевентс
description: Описывает метод List Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04197f9a6364cbd25816d4f860c2d57d94360fee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458233"
---
# <a name="list-mobileapptroubleshootingevents"></a>Список Мобилеапптраублешутинжевентс

Пространство имен: Microsoft. Graph

> **Важно!** API в версии/Beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
|&nbsp; &nbsp; **Управление устройствами**|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|&nbsp; &nbsp; **Устранение неполадок**|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений||
|&nbsp; &nbsp; **Управление устройствами**|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|&nbsp; &nbsp; **Устранение неполадок**|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents
GET /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
      "id": "77943c10-3c10-7794-103c-9477103c9477"
    }
  ]
}
```












