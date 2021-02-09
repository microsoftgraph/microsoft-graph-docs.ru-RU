---
title: Тип ресурса windowsAutopilotDeviceIdentity
description: Ресурс windowsAutopilotDeviceIdentity представляет устройство Windows Autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5bf74d47398fec117fa05a2fc3c81793af1aef9c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159544"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Тип ресурса windowsAutopilotDeviceIdentity

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс windowsAutopilotDeviceIdentity представляет устройство Windows Autopilot.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[Коллекция windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Список свойств и связей объектов [windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Get windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Чтение свойств и связей объекта [windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Создание объекта windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Создание объекта [windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Удаление объекта windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Нет|Удаляет объект [windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|
|[Действие assignUserToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Нет|Назначает пользователя устройствам Autopilot.|
|[Действие unassignUserFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Нет|Отписка пользователя с устройства Autopilot.|
|[Действие updateDeviceProperties](../api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties.md)|Нет|Обновляет свойства на устройствах Autopilot.|
|[Действие assignResourceAccountToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|Нет|Назначает учетную запись ресурса устройствам Autopilot.|
|[Действие unassignResourceAccountFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|Нет|Отписка учетной записи ресурса с устройства Autopilot.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Состояние назначения профиля устройства Windows Autopilot. Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Подробное состояние назначения профиля устройства Windows Autopilot. Возможные значения: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Время набора профилей устройства Windows Autopilot.|
|orderIdentifier|Строка|Order Identifier of the Windows autopilot device - Deprecated|
|groupTag|String|Тег группы устройства Windows Autopilot.|
|purchaseOrderIdentifier|String|Идентификатор заказа на покупку устройства Windows Autopilot.|
|serialNumber|Строка|Серийный номер устройства Windows Autopilot.|
|productKey|Строка|Ключ продукта устройства Windows Autopilot.|
|manufacturer|String|Изготовитель изготовителя устройства Windows Autopilot.|
|model|String|Имя модели устройства Windows Autopilot.|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние регистрации Устройства Windows Autopilot в Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|lastContactedDateTime|DateTimeOffset|Intune Last Contacted Date Time of the Windows autopilot device.|
|addressableUserName|String|Адресуемое имя пользователя.|
|userPrincipalName|String|Имя основного пользователя.|
|resourceName|String|Имя ресурса.|
|skuNumber|String|Номер SKU|
|systemFamily|String|Семейство систем|
|azureActiveDirectoryDeviceId|String|ИД устройства AAD|
|managedDeviceId|String|ИД управляемого устройства|
|displayName|String|"Display Name" (Отображаемое имя);|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Профиль развертывания, который в настоящее время назначен устройству Windows Autopilot.|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|Профиль развертывания, предназначенный для присвоения устройству Windows Autopilot.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "deploymentProfileAssignmentStatus": "String",
  "deploymentProfileAssignmentDetailedStatus": "String",
  "deploymentProfileAssignedDateTime": "String (timestamp)",
  "orderIdentifier": "String",
  "groupTag": "String",
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String",
  "resourceName": "String",
  "skuNumber": "String",
  "systemFamily": "String",
  "azureActiveDirectoryDeviceId": "String",
  "managedDeviceId": "String",
  "displayName": "String"
}
```




