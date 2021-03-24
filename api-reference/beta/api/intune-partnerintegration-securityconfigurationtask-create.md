---
title: Создание securityConfigurationTask
description: Создание нового объекта securityConfigurationTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4eb74131d95a15dd4cad64107d7452ca4cf9f071
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134832"
---
# <a name="create-securityconfigurationtask"></a>Создание securityConfigurationTask

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementApps.ReadWrite.All|

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
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта securityConfigurationTask.

В следующей таблице показаны свойства, необходимые при создании securityConfigurationTask.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ сущности. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|Строка|Имя. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|Строка|Описание. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|Дата создания. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|Срок действия. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|Категория. Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `unknown`, `advancedThreatProtection`.|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|Приоритет. Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `none`, `high`, `low`.|
|creator|Строка|Адрес электронной почты создателя. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|Строка|Заметки от создателя. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|Имя или электронная почта администратора этой задачи назначены. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|Состояние. Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.|
|endpointSecurityPolicy|[endpointSecurityConfigurationType](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|Тип политики безопасности конечной точки. Возможные значения: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.|
|applicablePlatform|[endpointSecurityConfigurationApplicablePlatform](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|Применимая платформа. Возможные значения: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.|
|endpointSecurityPolicyProfile|[endpointSecurityConfigurationProfileType](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|Профиль политики безопасности конечной точки. Возможные значения: `unknown` `antivirus` , , , , , `windowsSecurity` , `bitLocker` , `fileVault` `firewall` `firewallRules` `endpointDetectionAndResponse` `deviceControl` , `appAndBrowserIsolation` `exploitProtection` `webProtection` `applicationControl` `attackSurfaceReductionRules` `accountProtection` , .|
|insights|Строка|Сведения о смягчении последствий.|
|managedDeviceCount|Int32|Количество уязвимых устройств.|
|intendedSettings|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Предполагаемые параметры и их значения.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending",
  "endpointSecurityPolicy": "antivirus",
  "applicablePlatform": "macOS",
  "endpointSecurityPolicyProfile": "antivirus",
  "insights": "Insights value",
  "managedDeviceCount": 2,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 854

{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "id": "5d630f12-0f12-5d63-120f-635d120f635d",
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
  "endpointSecurityPolicy": "antivirus",
  "applicablePlatform": "macOS",
  "endpointSecurityPolicyProfile": "antivirus",
  "insights": "Insights value",
  "managedDeviceCount": 2,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ]
}
```




