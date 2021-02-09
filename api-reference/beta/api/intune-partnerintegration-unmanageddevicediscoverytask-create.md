---
title: Создание unmanagedDeviceDiscoveryTask
description: Создание объекта unmanagedDeviceDiscoveryTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 065412c80272f6d3f87b00497365069cab923271
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162602"
---
# <a name="create-unmanageddevicediscoverytask"></a>Создание unmanagedDeviceDiscoveryTask

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/deviceAppManagementTasks
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта unmanagedDeviceDiscoveryTask в JSON.

В следующей таблице показаны свойства, необходимые при создании объекта unmanagedDeviceDiscoveryTask.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|Имя. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|String|Описание. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|Дата создания. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|Дата окончания. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|Категория. Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md) Возможные значения: `unknown`, `advancedThreatProtection`.|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|Приоритет. Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md) Возможные значения: `none`, `high`, `low`.|
|creator|String|Адрес электронной почты создателя. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|String|Примечания от создателя. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|Имя или адрес электронной почты администратора, для которого назначена эта задача. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|Состояние. Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md) Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.|
|unmanagedDevices|[коллекция unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)|Неугодные устройства, обнаруженные в сети.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и объект `201 Created` [unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
Content-type: application/json
Content-length: 961

{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "Os value",
      "osVersion": "Os Version value",
      "ipAddress": "Ip Address value",
      "deviceName": "Device Name value",
      "macAddress": "Mac Address value",
      "domain": "Domain value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "location": "Location value",
      "lastLoggedOnUser": "Last Logged On User value",
      "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
    }
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "id": "6caa2ba0-2ba0-6caa-a02b-aa6ca02baa6c",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "Os value",
      "osVersion": "Os Version value",
      "ipAddress": "Ip Address value",
      "deviceName": "Device Name value",
      "macAddress": "Mac Address value",
      "domain": "Domain value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "location": "Location value",
      "lastLoggedOnUser": "Last Logged On User value",
      "lastSeenDateTime": "2017-01-01T00:02:00.1006212-08:00"
    }
  ]
}
```




