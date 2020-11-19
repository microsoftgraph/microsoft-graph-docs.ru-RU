---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62c4b0684f7e72b2dbba6ed840e7b5d8785d0dc9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261113"
---
# <a name="mobileapprelationshipstate-resource-type"></a>Тип ресурса Мобилеаппрелатионшипстате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|саурцеидс|Коллекция строк|Коллекция идентификаторов исходного приложения для мобильных устройств.|
|targetId|String|Идентификатор связанного конечного приложения.|
|таржетдисплайнаме|String|Отображаемое имя связанного конечного приложения.|
|deviceId|String|Соответствующий идентификатор устройства.|
|installState|[ресултантаппстате](../resources/intune-shared-resultantappstate.md)|Состояние установки приложения конечного приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|инсталлстатедетаил|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Сведения о состоянии установки приложения. Возможные значения:,,,,,,,,,,,,,,,,,, `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` , `seeUninstallErrorCode` , `pendingReboot` , `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` ,,,,,,,,,,,,,,,,,.|
|errorCode|Int32|Код ошибки для установки или удаления сбоев конечного приложения.|
|таржетластсинкдатетиме|DateTimeOffset|Время последней синхронизации конечного приложения.|

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




