---
title: Тип ресурса remoteActionAudit
description: Отчет о удаленного действия, которые запускаются на устройствах, относящегося к определенной клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ebe93b2f2e70011fb75a08b91938f26d723d1d5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404913"
---
# <a name="remoteactionaudit-resource-type"></a>Тип ресурса remoteActionAudit

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отчет о удаленного действия, которые запускаются на устройствах, относящегося к определенной клиента.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список remoteActionAudits](../api/intune-devices-remoteactionaudit-list.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) коллекции|Свойства списка и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Получение remoteActionAudit](../api/intune-devices-remoteactionaudit-get.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Чтение свойства и связи объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Создание remoteActionAudit](../api/intune-devices-remoteactionaudit-create.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|
|[Удаление remoteActionAudit](../api/intune-devices-remoteactionaudit-delete.md)|Нет|Удаляет [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).|
|[Обновление remoteActionAudit](../api/intune-devices-remoteactionaudit-update.md)|[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)|Обновление свойства объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор отчета.|
|deviceDisplayName|String|Имя устройства Intune.|
|userName|String|\[устаревшие\] вместо этого используйте InitiatedByUserPrincipalName.|
|initiatedByUserPrincipalName|String|Пользователя, который инициировал действие устройства имеет формат имени участника-пользователя.|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|Имя действия. Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .|
|requestDateTime|DateTimeOffset|Время, когда действие был отправлен, в формате UTC.|
|deviceOwnerUserPrincipalName|String|Имя участника-пользователя владельца устройства.|
|deviceIMEI|String|IMEI устройства.|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|

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
  "actionState": "String"
}
```




