---
title: Обновление securityConfigurationTask
description: Обновление свойств объекта securityConfigurationTask.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da676753f8070f94aaa6c1b7902899d299e2fee0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59092695"
---
# <a name="update-securityconfigurationtask"></a>Обновление securityConfigurationTask

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)

## <a name="prerequisites"></a>Необходимые компоненты
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
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)

В следующей таблице показаны свойства, необходимые при создании [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|Имя. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|String|Описание. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|Дата создания. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|Срок действия. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|Категория. Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `unknown`, `advancedThreatProtection`.|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|Приоритет. Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `none`, `high`, `low`.|
|creator|String|Адрес электронной почты создателя. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|String|Заметки от создателя. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|Имя или электронная почта администратора этой задачи назначены. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|Состояние. Унаследовано от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.|
|endpointSecurityPolicy|[endpointSecurityConfigurationType](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|Тип политики безопасности конечной точки. Возможные значения: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.|
|applicablePlatform|[endpointSecurityConfigurationApplicablePlatform](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|Применимая платформа. Возможные значения: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.|
|endpointSecurityPolicyProfile|[endpointSecurityConfigurationProfileType](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|Профиль политики безопасности конечной точки. Возможные значения: `unknown` `antivirus` , , , , , `windowsSecurity` , `bitLocker` , `fileVault` `firewall` `firewallRules` `endpointDetectionAndResponse` `deviceControl` , `appAndBrowserIsolation` `exploitProtection` `webProtection` `applicationControl` `attackSurfaceReductionRules` `accountProtection` , .|
|insights|String|Сведения о смягчении последствий.|
|managedDeviceCount|Int32|Количество уязвимых устройств.|
|intendedSettings|Коллекция [keyValuePair](../resources/intune-partnerintegration-keyvaluepair.md)|Предполагаемые параметры и их значения.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
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
HTTP/1.1 200 OK
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



