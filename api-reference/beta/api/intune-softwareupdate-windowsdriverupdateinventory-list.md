---
title: Список windowsDriverUpdateInventories
description: Список свойств и связей объектов WindowsDriverUpdateInventory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7a6d863ec480ae60beb9bf02687552ca5573766c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344276"
---
# <a name="list-windowsdriverupdateinventories"></a>Список windowsDriverUpdateInventories

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей [объектов WindowsDriverUpdateInventory.](../resources/intune-softwareupdate-windowsdriverupdateinventory.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/driverInventories
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [WindowsDriverUpdateInventory](../resources/intune-softwareupdate-windowsdriverupdateinventory.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/driverInventories
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDriverUpdateInventory",
      "id": "3b14b403-b403-3b14-03b4-143b03b4143b",
      "name": "Name value",
      "version": "Version value",
      "manufacturer": "Manufacturer value",
      "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
      "driverClass": "Driver Class value",
      "applicableDeviceCount": 5,
      "approvalStatus": "declined",
      "category": "previouslyApproved",
      "deployDateTime": "2017-01-01T00:01:14.7822152-08:00"
    }
  ]
}
```




