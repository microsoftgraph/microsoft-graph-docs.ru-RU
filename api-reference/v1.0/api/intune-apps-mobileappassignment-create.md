---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc9fd43ae46e66772eae5ef6a492cae9802692fc
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730527"
---
# <a name="create-mobileappassignment"></a>Создание объекта mobileAppAssignment

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.

В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|intent|[installIntent](../resources/intune-shared-installintent.md)|Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевое назначение группы, определенное администратором.|
|settings|[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)|Параметры целевого назначения, определенные администратором.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 861

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings",
    "notifications": "showReboot",
    "restartSettings": {
      "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
      "gracePeriodInMinutes": 4,
      "countdownDisplayBeforeRestartInMinutes": 6,
      "restartNotificationSnoozeDurationInMinutes": 10
    },
    "installTimeSettings": {
      "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
      "useLocalTime": true,
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "deadlineDateTime": "2017-01-01T00:00:21.0378955-08:00"
    },
    "deliveryOptimizationPriority": "foreground"
  }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 910

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings",
    "notifications": "showReboot",
    "restartSettings": {
      "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
      "gracePeriodInMinutes": 4,
      "countdownDisplayBeforeRestartInMinutes": 6,
      "restartNotificationSnoozeDurationInMinutes": 10
    },
    "installTimeSettings": {
      "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
      "useLocalTime": true,
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "deadlineDateTime": "2017-01-01T00:00:21.0378955-08:00"
    },
    "deliveryOptimizationPriority": "foreground"
  }
}
```





