---
title: Тип ресурса remoteActionAudit
description: Отчет о удаленных действиях, запущенных на устройствах, относящихся к определенному клиенту.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70a4a95019db6ca3025d0090981ca6563d335ffe
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804265"
---
# <a name="remoteactionaudit-resource-type"></a>Тип ресурса remoteActionAudit

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|action|[Ремотеактион](../resources/intune-devices-remoteaction.md)|Имя действия. Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `logoutSharedAppleDeviceActiveUser` `quickScan`,,,,,,,,,,,,,,,,,,,,, `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` .|
|Рекуестдатетиме|DateTimeOffset|Время, когда действие было выдано, заданное в формате UTC.|
|deviceOwnerUserPrincipalName|String|Имя участника-пользователя для владельца устройства.|
|deviceIMEI|String|IMEI устройства.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|

## <a name="relationships"></a>Отношения
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
  "actionState": "String"
}
```





