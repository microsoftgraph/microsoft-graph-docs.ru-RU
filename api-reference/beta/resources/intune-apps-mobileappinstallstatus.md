---
title: тип ресурса mobileAppInstallStatus
description: Содержит свойства для состояния установки мобильного приложения для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3df7c22b137e1a3b866b425bb8b355024c3f63e5
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262767"
---
# <a name="mobileappinstallstatus-resource-type"></a>тип ресурса mobileAppInstallStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния установки мобильного приложения для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileAppInstallStatuses](../api/intune-apps-mobileappinstallstatus-list.md)|[коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список свойств и связей объектов [mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)|
|[Get mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Чтение свойств и связей объекта [mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)|
|[Создание mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Создание нового [объекта mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)|
|[Удаление mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-delete.md)|Нет|Удаляет [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).|
|[Обновление mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Обновление свойств объекта [mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|deviceName|String|Имя устройства|
|deviceId|String|ID устройства|
|lastSyncDateTime|DateTimeOffset|Время последней даты синхронизации|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-apps-resultantappstate.md)|Состояние установки приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installState|[resultantAppState](../resources/intune-apps-resultantappstate.md)|Состояние установки приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Деталь состояния установки приложения. Возможные значения: `noAdditionalDetails` `dependencyFailedToInstall` , `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` , `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` , .|
|errorCode|Int32|Код ошибки для установки или отказа от сбоев.|
|osVersion|String|ВЕРСИЯ ОС|
|osDescription|String|Описание ОС|
|userName|String|Имя пользователя устройства|
|userPrincipalName|String|"User Principal Name" (Имя участника-пользователя);|
|displayVersion|Строка|Читаемая для человека версия приложения|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|приложение|[mobileApp](../resources/intune-shared-mobileapp.md);|Ссылка на навигацию в мобильном приложении.|

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




