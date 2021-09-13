---
title: тип ресурса remoteActionAudit
description: Отчет о удаленных действиях, инициированных на устройствах, принадлежащих определенному клиенту.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd3e1acabcc5c4e51a4febb307eb0084e1f03292
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081082"
---
# <a name="remoteactionaudit-resource-type"></a>тип ресурса remoteActionAudit

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отчет о удаленных действиях, инициированных на устройствах, принадлежащих определенному клиенту.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|[коллекция remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Список свойств и связей объектов [remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)|
|[Get remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Чтение свойств и связей объекта [remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)|
|[Создание remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Создание нового [объекта remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)|
|[Удаление remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|Нет|Удаляет [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).|
|[Обновление remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Обновление свойств объекта [remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Report Id.|
|deviceDisplayName|String|Имя устройства Intune.|
|userName|String|\[deprecated \] Please use InitiatedByUserPrincipalName instead.|
|initiatedByUserPrincipalName|String|Пользователь, который инициировал действие устройства, формат upN.|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|Имя действия. Возможные значения: `unknown` `factoryReset` , , `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` . `setDeviceName` `activateDeviceEsim`|
|requestDateTime|DateTimeOffset|Время, когда действие было выдано, дано в UTC.|
|deviceOwnerUserPrincipalName|String|Upn владельца устройства.|
|deviceIMEI|String|IMEI устройства.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|managedDeviceId|String|Цель действия.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String",
  "managedDeviceId": "String"
}
```



