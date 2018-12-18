---
title: Тип ресурса remoteActionAudit
description: Отчет о удаленного действия, которые запускаются на устройствах, относящегося к определенной клиента.
author: tfitzmac
ms.openlocfilehash: 48d74cb088a2e16e244898834e3d717302713e6f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323480"
---
# <a name="remoteactionaudit-resource-type"></a>Тип ресурса remoteActionAudit

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|id|Строка|Идентификатор отчета.|
|deviceDisplayName|String|Имя устройства Intune.|
|userName|String|\[устаревшие\] вместо этого используйте InitiatedByUserPrincipalName.|
|initiatedByUserPrincipalName|String.|Пользователя, который инициировал действие устройства имеет формат имени участника-пользователя.|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|Имя действия. Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .|
|requestDateTime|DateTimeOffset|Время, когда действие был отправлен, в формате UTC.|
|deviceOwnerUserPrincipalName|String.|Имя участника-пользователя владельца устройства.|
|deviceIMEI|String.|IMEI устройства.|
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





