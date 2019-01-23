---
title: Тип ресурса windowsAutopilotDeviceIdentity
description: Ресурс windowsAutopilotDeviceIdentity представляет автопилот устройства Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e69f93aff041f99728a224ce6e50a5e711919b1e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423925"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Тип ресурса windowsAutopilotDeviceIdentity

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс windowsAutopilotDeviceIdentity представляет автопилот устройства Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) коллекции|Свойства списка и связей объектов [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Получение windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Чтение свойства и связи объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Создание windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Удаление windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Нет|Удаляет [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).|
|[Обновление windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Обновление свойства объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Действие assignUserToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Нет|Назначает пользователю на автопилот устройства.|
|[Действие unassignUserFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Нет|Unassigns пользователя из устройства автопилот.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Состояние назначения профиля устройства автопилот Windows. Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Назначение профиля подробное описание состояния устройства автопилот Windows. Возможные значения: `none`, `hardwareRequirementsNotMet`.|
|deploymentProfileAssignedDateTime|DateTimeOffset|Профиль задания времени автопилот устройства Windows.|
|orderIdentifier|Строка|Порядок идентификатор устройства автопилот Windows.|
|purchaseOrderIdentifier|String|Идентификатор заказа на покупку автопилот устройства Windows.|
|serialNumber|Строка|Серийный номер устройства Windows Autopilot.|
|productKey|Строка|Ключ продукта устройства Windows Autopilot.|
|manufacturer|String|Изготовителей автопилот устройства Windows.|
|model|String|Имя модели устройства автопилот Windows.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Состояние регистрации автопилот устройства Windows Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|lastContactedDateTime|DateTimeOffset|Intune связаться с даты последнего устройства автопилот Windows.|
|addressableUserName|String|Имя адресации пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|В настоящее время назначены устройства Windows автопилот профиль развертывания.|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Профиля развертывания предназначен для назначения автопилот устройства Windows.|

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
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String"
}
```




