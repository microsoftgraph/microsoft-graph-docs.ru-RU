---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 116e57ba4bad4474e8ec28bda990ac9e2fe1df86
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076352"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="5484b-103">Тип ресурса Мобилеаппрелатионшипстате</span><span class="sxs-lookup"><span data-stu-id="5484b-103">mobileAppRelationshipState resource type</span></span>

<span data-ttu-id="5484b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5484b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5484b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5484b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5484b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5484b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5484b-107">Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.</span><span class="sxs-lookup"><span data-stu-id="5484b-107">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="5484b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5484b-108">Properties</span></span>
|<span data-ttu-id="5484b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5484b-109">Property</span></span>|<span data-ttu-id="5484b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5484b-110">Type</span></span>|<span data-ttu-id="5484b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5484b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5484b-112">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="5484b-112">sourceIds</span></span>|<span data-ttu-id="5484b-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5484b-113">String collection</span></span>|<span data-ttu-id="5484b-114">Коллекция идентификаторов исходного приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="5484b-114">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="5484b-115">targetId</span><span class="sxs-lookup"><span data-stu-id="5484b-115">targetId</span></span>|<span data-ttu-id="5484b-116">String</span><span class="sxs-lookup"><span data-stu-id="5484b-116">String</span></span>|<span data-ttu-id="5484b-117">Идентификатор связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="5484b-117">The related target app's id.</span></span>|
|<span data-ttu-id="5484b-118">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="5484b-118">targetDisplayName</span></span>|<span data-ttu-id="5484b-119">String</span><span class="sxs-lookup"><span data-stu-id="5484b-119">String</span></span>|<span data-ttu-id="5484b-120">Отображаемое имя связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="5484b-120">The related target app's display name.</span></span>|
|<span data-ttu-id="5484b-121">deviceId</span><span class="sxs-lookup"><span data-stu-id="5484b-121">deviceId</span></span>|<span data-ttu-id="5484b-122">String</span><span class="sxs-lookup"><span data-stu-id="5484b-122">String</span></span>|<span data-ttu-id="5484b-123">Соответствующий идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="5484b-123">The corresponding device id.</span></span>|
|<span data-ttu-id="5484b-124">installState</span><span class="sxs-lookup"><span data-stu-id="5484b-124">installState</span></span>|[<span data-ttu-id="5484b-125">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="5484b-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="5484b-126">Состояние установки приложения конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="5484b-126">The install state of the app of target app.</span></span> <span data-ttu-id="5484b-127">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="5484b-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="5484b-128">инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="5484b-128">installStateDetail</span></span>|[<span data-ttu-id="5484b-129">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="5484b-129">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="5484b-130">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="5484b-130">The install state detail of the app.</span></span> <span data-ttu-id="5484b-131">Возможные значения:,,,,,,,,,,,,,,,,,, `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` , `seeUninstallErrorCode` , `pendingReboot` , `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` ,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="5484b-131">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="5484b-132">errorCode</span><span class="sxs-lookup"><span data-stu-id="5484b-132">errorCode</span></span>|<span data-ttu-id="5484b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5484b-133">Int32</span></span>|<span data-ttu-id="5484b-134">Код ошибки для установки или удаления сбоев конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="5484b-134">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="5484b-135">таржетластсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="5484b-135">targetLastSyncDateTime</span></span>|<span data-ttu-id="5484b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5484b-136">DateTimeOffset</span></span>|<span data-ttu-id="5484b-137">Время последней синхронизации конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="5484b-137">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5484b-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="5484b-138">Relationships</span></span>
<span data-ttu-id="5484b-139">Нет</span><span class="sxs-lookup"><span data-stu-id="5484b-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5484b-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5484b-140">JSON Representation</span></span>
<span data-ttu-id="5484b-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5484b-141">Here is a JSON representation of the resource.</span></span>
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






