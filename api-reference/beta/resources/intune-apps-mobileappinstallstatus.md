---
title: Тип ресурса mobileAppInstallStatus
description: Содержит свойства для установки состояния мобильного приложения для устройства.
ms.openlocfilehash: efd5969e2c00d0230d8efeddff3c41bac90fe9c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076850"
---
# <a name="mobileappinstallstatus-resource-type"></a>Тип ресурса mobileAppInstallStatus

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для установки состояния мобильного приложения для устройства.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) коллекции|Свойства списка и связей объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Получение mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Чтение свойства и связи объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Создание mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Создание нового объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Удаление mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-delete.md)|Нет|Удаляет [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).|
|[Обновление mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Обновление свойства объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|deviceName|String|Имя устройства|
|deviceId|String|Идентификатор устройства|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-shared-resultantappstate.md)|Состояние установки приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installState|[resultantAppState](../resources/intune-shared-resultantappstate.md)|Состояние установки приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Сведений о состоянии установки приложения. Возможные значения: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|errorCode|Int32|Сообщение об ошибке примеры кода для установки или удаления сбоев.|
|osVersion|String|Версия операционной системы|
|osDescription|String|Описание операционная система|
|userName|String|Имя пользователя устройства|
|userPrincipalName|String|"User Principal Name" (Имя участника-пользователя);|
|displayVersion|String|Человеческого для чтения версию приложения|

## <a name="relationships"></a>Связи
|Связь|Тип|Description|
|:---|:---|:---|
|приложение|[mobileApp](../resources/intune-apps-mobileapp.md);|Навигационная ссылка для мобильного приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "displayVersion": "String"
}
```





