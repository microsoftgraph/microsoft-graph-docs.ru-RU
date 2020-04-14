---
title: Тип ресурса remoteActionAudit
description: Отчет о удаленных действиях, запущенных на устройствах, относящихся к определенному клиенту.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab0ada68ca9d11b4c2a1c9ec7962a34f5cc665eb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446958"
---
# <a name="remoteactionaudit-resource-type"></a>Тип ресурса remoteActionAudit

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отчет о удаленных действиях, запущенных на устройствах, относящихся к определенному клиенту.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Ремотеактионаудитс](../api/intune-devices-remoteactionaudit-list.md)|Коллекция [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Список свойств и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Получение remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Чтение свойств и связей объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Создание remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Удаление remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|Нет|Удаляет объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).|
|[Обновление remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Обновление свойств объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор отчета.|
|deviceDisplayName|String|Имя устройства Intune.|
|userName|String|\[\] рекомендуется вместо этого использовать свойства initiatedbyuserprincipalname.|
|Свойства initiatedbyuserprincipalname|String|Пользователь, который инициировал действие с устройством, имеет формат UPN.|
|action|[ремотеактион](../resources/intune-devices-remoteaction.md)|Имя действия. Возможные `unknown`значения:, `factoryReset`, `removeCompanyData`, `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName`,,,,,,, `quickScan`,,,,,,,,,,,,,,,,,,. `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser`|
|рекуестдатетиме|DateTimeOffset|Время, когда действие было выдано, заданное в формате UTC.|
|deviceOwnerUserPrincipalName|String|Имя участника-пользователя для владельца устройства.|
|deviceIMEI|String|IMEI устройства.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|манажеддевицеид|String|Цель действия.|

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



