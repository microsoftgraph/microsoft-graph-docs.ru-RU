---
title: тип ресурса remoteActionAudit
description: Отчет о удаленных действиях, инициированных на устройствах, принадлежащих определенному клиенту.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3cf9a0c16063c0f2fcd359598a677fa59ad042f49472077be354bc40854ed75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249869"
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
|initiatedByUserPrincipalName|Строка|Пользователь, который инициировал действие устройства, формат upN.|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|Имя действия. Возможные значения: `unknown` `factoryReset` , , `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` . `setDeviceName` `activateDeviceEsim`|
|requestDateTime|DateTimeOffset|Время, когда действие было выдано, дано в UTC.|
|deviceOwnerUserPrincipalName|Строка|Upn владельца устройства.|
|deviceIMEI|Строка|IMEI устройства.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|managedDeviceId|Строка|Цель действия.|

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




