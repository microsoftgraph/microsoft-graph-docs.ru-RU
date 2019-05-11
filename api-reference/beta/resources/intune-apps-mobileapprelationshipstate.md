---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35080ad21137387fb63ff2fcb22233ff1be74cde
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949894"
---
# <a name="mobileapprelationshipstate-resource-type"></a>Тип ресурса Мобилеаппрелатионшипстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Саурцеидс|Коллекция строк|Коллекция идентификаторов исходного приложения для мобильных устройств.|
|targetId|Строка|Идентификатор связанного конечного приложения.|
|Таржетдисплайнаме|Строка|Отображаемое имя связанного конечного приложения.|
|deviceId|String|Соответствующий идентификатор устройства.|
|installState|[Ресултантаппстате](../resources/intune-shared-resultantappstate.md)|Состояние установки приложения конечного приложения. Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|Инсталлстатедетаил|[resultantAppStateDetail](../resources/intune-apps-resultantappstatedetail.md)|Сведения о состоянии установки приложения. Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`,,,,,,,,,,,,,,,,,,,,, `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` , `processorArchitectureNotApplicable`.|
|errorCode|Int32|Код ошибки для установки или удаления сбоев конечного приложения.|
|Таржетластсинкдатетиме|DateTimeOffset|Время последней синхронизации конечного приложения.|

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




