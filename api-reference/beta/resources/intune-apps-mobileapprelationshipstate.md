---
title: тип ресурса mobileAppRelationshipState
description: Описывает сведения о состоянии установки детского приложения в контексте upN и id устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58927afdfce4336eb3d0abfcf234f9c1dc1fe77e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803043"
---
# <a name="mobileapprelationshipstate-resource-type"></a>тип ресурса mobileAppRelationshipState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает сведения о состоянии установки детского приложения в контексте upN и id устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|sourceIds|Коллекция String|Коллекция исходных ids мобильного приложения.|
|targetId|Строка|ID связанного целевого приложения.|
|targetDisplayName|Строка|Имя отображения связанного целевого приложения.|
|deviceId|String|Соответствующий id устройства.|
|installState|[resultantAppState](../resources/intune-apps-resultantappstate.md)|Состояние установки приложения целевого приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Деталь состояния установки приложения. Возможные значения: `noAdditionalDetails` `dependencyFailedToInstall` , `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `supersededAppUninstallFailed` `supersededAppUninstallPendingReboot` `removingSupersededApps` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `uninstallPendingReboot` `supersedingAppsDetected` `supersededAppsDetected` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `untargetedSupersedingAppsDetected` `appRemovedBySupersedence` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `supersedingAppsNotApplicable` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` . `processorArchitectureNotApplicable`|
|errorCode|Int32|Код ошибки для установки или сбои в целевом приложении.|
|targetLastSyncDateTime|DateTimeOffset|Последнее время синхронизации целевого приложения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppRelationshipState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationshipState",
  "sourceIds": [
    "String"
  ],
  "targetId": "String",
  "targetDisplayName": "String",
  "deviceId": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 1024,
  "targetLastSyncDateTime": "String (timestamp)"
}
```



