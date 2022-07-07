---
title: Тип ресурса mobileAppInstallStatus
description: Содержит свойства для состояния установки мобильного приложения для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: efcf9d78aecd7ba49e5630473e790d3ed7c37406
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671235"
---
# <a name="mobileappinstallstatus-resource-type"></a>Тип ресурса mobileAppInstallStatus

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния установки мобильного приложения для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов mobileAppInstallStatuse](../api/intune-apps-mobileappinstallstatus-list.md)|[Коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Список свойств и связей объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Получение объекта mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-get.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Чтение свойств и связей объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Создание объекта mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-create.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Создайте объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|
|[Удаление mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-delete.md)|Нет|Удаляет [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).|
|[Обновление mobileAppInstallStatus](../api/intune-apps-mobileappinstallstatus-update.md)|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Обновление свойств объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|deviceName|String|Имя устройства|
|deviceId|String|Код устройства|
|lastSyncDateTime|DateTimeOffset|Дата последней синхронизации|
|mobileAppInstallStatusValue|[resultantAppState](../resources/intune-apps-resultantappstate.md)|Состояние установки приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installState|[resultantAppState](../resources/intune-apps-resultantappstate.md)|Состояние установки приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Сведения о состоянии установки приложения. Возможные значения: `noAdditionalDetails`, , `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet``dependencyPendingReboot``dependencyWithAutoInstallDisabled``supersededAppUninstallFailed``supersededAppUninstallPendingReboot``removingSupersededApps``iosAppStoreUpdateFailedToInstall``vppAppHasUpdateAvailable``userRejectedUpdate``uninstallPendingReboot``supersedingAppsDetected``supersededAppsDetected``seeInstallErrorCode``autoInstallDisabled``managedAppNoLongerPresent``userRejectedInstall``userIsNotLoggedIntoAppStore``untargetedSupersedingAppsDetected``appRemovedBySupersedence``seeUninstallErrorCode``pendingReboot``installingDependencies``contentDownloaded``supersedingAppsNotApplicable``powerShellScriptRequirementNotMet``registryRequirementNotMet``fileSystemRequirementNotMet``platformNotApplicable``minimumCpuSpeedNotMet``minimumLogicalProcessorCountNotMet``minimumPhysicalMemoryNotMet``minimumOsVersionNotMet``minimumDiskSpaceNotMet``processorArchitectureNotApplicable`|
|errorCode|Int32|Код ошибки для сбоев установки или удаления.|
|osVersion|String|Версия ОС|
|osDescription|String|Описание ОС|
|userName|String|Имя пользователя устройства|
|userPrincipalName|String|"User Principal Name" (Имя участника-пользователя);|
|displayVersion|String|Удобочитаемая версия приложения|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|приложение|[mobileApp](../resources/intune-apps-mobileapp.md);|Навигационная ссылка на мобильное приложение.|

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




