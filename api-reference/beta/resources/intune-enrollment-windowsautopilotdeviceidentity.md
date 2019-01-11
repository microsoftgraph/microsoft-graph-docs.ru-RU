---
title: Тип ресурса windowsAutopilotDeviceIdentity
description: Ресурс windowsAutopilotDeviceIdentity представляет автопилот устройства Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9fd7ac1f6cc97c16fc5ab393cc9b893386eb9e65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851157"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Тип ресурса windowsAutopilotDeviceIdentity

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|purchaseOrderIdentifier|Строка|Идентификатор заказа на покупку автопилот устройства Windows.|
|serialNumber|Строка|Серийный номер устройства Windows Autopilot.|
|productKey|Строка|Ключ продукта устройства Windows Autopilot.|
|manufacturer|String|Изготовителей автопилот устройства Windows.|
|model|String|Имя модели устройства автопилот Windows.|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Состояние регистрации автопилот устройства Windows Intune. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|lastContactedDateTime|DateTimeOffset|Intune связаться с даты последнего устройства автопилот Windows.|
|addressableUserName|Строка|Имя адресации пользователя.|
|userPrincipalName|Строка|Имя участника-пользователя.|

## <a name="relationships"></a>Связи
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





