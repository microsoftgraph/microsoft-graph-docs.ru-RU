---
title: тип ресурса securityConfigurationTask
description: Задача конфигурации безопасности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 619cd0c8ad95f8791d103cf70996e1181e3d0f78
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789223"
---
# <a name="securityconfigurationtask-resource-type"></a>тип ресурса securityConfigurationTask

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Задача конфигурации безопасности.


Наследует [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List securityConfigurationTasks](../api/intune-partnerintegration-securityconfigurationtask-list.md)|[коллекция securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Список свойств и связей объектов [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)|
|[Получить securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-get.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Чтение свойств и связей объекта [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)|
|[Создание securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-create.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Создание нового [объекта securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)|
|[Удаление securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-delete.md)|Нет|Удаляет [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md).|
|[Обновление securityConfigurationTask](../api/intune-partnerintegration-securityconfigurationtask-update.md)|[securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md)|Обновление свойств объекта [securityConfigurationTask.](../resources/intune-partnerintegration-securityconfigurationtask.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|Имя. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|String|Описание. Унаследованный от [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
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
|insights|String|Сведения о смягчении последствий.|
|managedDeviceCount|Int32|Количество уязвимых устройств.|
|intendedSettings|Коллекция [keyValuePair](../resources/intune-partnerintegration-keyvaluepair.md)|Предполагаемые параметры и их значения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevices|[vulnerableManagedDevice collection](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Уязвимые управляемые устройства.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityConfigurationTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String",
  "endpointSecurityPolicy": "String",
  "applicablePlatform": "String",
  "endpointSecurityPolicyProfile": "String",
  "insights": "String",
  "managedDeviceCount": 1024,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



