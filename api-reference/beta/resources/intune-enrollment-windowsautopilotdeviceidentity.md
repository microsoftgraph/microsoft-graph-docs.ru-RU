---
title: Тип ресурса windowsAutopilotDeviceIdentity
description: Ресурс windowsAutopilotDeviceIdentity представляет устройство автопилота Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5729c1b47a56f06ffd931df66b2c0ae1d76adc5b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547097"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>Тип ресурса windowsAutopilotDeviceIdentity

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс windowsAutopilotDeviceIdentity представляет устройство автопилота Windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсаутопилотдевицеидентитиес](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|Коллекция [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Список свойств и связей объектов [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Получение windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Чтение свойств и связей объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Создание windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Удаление windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|Нет|Удаляет объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).|
|[Обновление windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|Обновление свойств объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .|
|[Действие assignUserToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|Нет|Назначение пользователям автопилотных устройств.|
|[Действие unassignUserFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|Нет|Отменяет назначение пользователя для автопилотного устройства.|
|[Действие assignResourceAccountToDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|Нет|Назначение учетной записи ресурса автопилотным устройствам.|
|[Действие unassignResourceAccountFromDevice](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|Нет|Отменяет назначение учетной записи ресурса для автопилотного устройства.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|Деплойментпрофилеассигнментстатус|[Виндовсаутопилотпрофилеассигнментстатус](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Состояние назначения профиля устройства автопилота Windows. Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.|
|Деплойментпрофилеассигнментдетаиледстатус|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|Подробное состояние назначения профиля для устройства автопилота Windows. Возможные значения: `none`, `hardwareRequirementsNotMet`.|
|Деплойментпрофилеассигнеддатетиме|DateTimeOffset|Время настройки профиля для устройства автопилота Windows.|
|orderIdentifier|String|Идентификатор заказа устройства с автопилотом Windows — не является устаревшим|
|Грауптаг|String|Тег Group для устройства автопилота Windows.|
|Пурчасеордеридентифиер|String|Идентификатор заказа на покупку для устройства автопилота Windows.|
|serialNumber|String|Серийный номер устройства Windows Autopilot.|
|productKey|Строка|Ключ продукта устройства Windows Autopilot.|
|manufacturer|String|OEM-производитель устройства автопилота Windows.|
|model|String|Имя модели для устройства автопилота Windows.|
|Енроллментстате|[Енроллментстате](../resources/intune-enrollment-enrollmentstate.md)|Состояние регистрации в Intune для устройства автопилота Windows. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|Ластконтактеддатетиме|DateTimeOffset|Дата и время последнего обращения в Intune к устройству автопилота Windows.|
|Аддрессаблеусернаме|String|Имя пользователя с адресом.|
|userPrincipalName|String|Имя участника пользователя.|
|resourceName|String|Имя ресурса.|
|Скунумбер|String|Номер SKU|
|Системфамили|String|Семейство системы|
|Свойства azureactivedirectorydeviceid|String|ИДЕНТИФИКАТОР устройства AAD|
|Манажеддевицеид|String|Управляемый идентификатор устройства|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|Деплойментпрофиле|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Профиль развертывания, назначенный устройству автопилота Windows в настоящее время.|
|Интендеддеплойментпрофиле|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Профиль развертывания предназначен для назначения устройству автопилота Windows.|

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
  "managedDeviceId": "String"
}
```





