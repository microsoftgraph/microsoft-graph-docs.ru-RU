---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a417d655970147f7d6352c6d0c9624888a5da583
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48719745"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="ca651-103">Тип ресурса Мобилеаппрелатионшипстате</span><span class="sxs-lookup"><span data-stu-id="ca651-103">mobileAppRelationshipState resource type</span></span>

<span data-ttu-id="ca651-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca651-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca651-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca651-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca651-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca651-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca651-107">Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.</span><span class="sxs-lookup"><span data-stu-id="ca651-107">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="ca651-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca651-108">Properties</span></span>
|<span data-ttu-id="ca651-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca651-109">Property</span></span>|<span data-ttu-id="ca651-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ca651-110">Type</span></span>|<span data-ttu-id="ca651-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca651-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca651-112">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="ca651-112">sourceIds</span></span>|<span data-ttu-id="ca651-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ca651-113">String collection</span></span>|<span data-ttu-id="ca651-114">Коллекция идентификаторов исходного приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="ca651-114">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="ca651-115">targetId</span><span class="sxs-lookup"><span data-stu-id="ca651-115">targetId</span></span>|<span data-ttu-id="ca651-116">Строка</span><span class="sxs-lookup"><span data-stu-id="ca651-116">String</span></span>|<span data-ttu-id="ca651-117">Идентификатор связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ca651-117">The related target app's id.</span></span>|
|<span data-ttu-id="ca651-118">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="ca651-118">targetDisplayName</span></span>|<span data-ttu-id="ca651-119">Строка</span><span class="sxs-lookup"><span data-stu-id="ca651-119">String</span></span>|<span data-ttu-id="ca651-120">Отображаемое имя связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ca651-120">The related target app's display name.</span></span>|
|<span data-ttu-id="ca651-121">deviceId</span><span class="sxs-lookup"><span data-stu-id="ca651-121">deviceId</span></span>|<span data-ttu-id="ca651-122">String</span><span class="sxs-lookup"><span data-stu-id="ca651-122">String</span></span>|<span data-ttu-id="ca651-123">Соответствующий идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="ca651-123">The corresponding device id.</span></span>|
|<span data-ttu-id="ca651-124">installState</span><span class="sxs-lookup"><span data-stu-id="ca651-124">installState</span></span>|[<span data-ttu-id="ca651-125">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="ca651-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ca651-126">Состояние установки приложения конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ca651-126">The install state of the app of target app.</span></span> <span data-ttu-id="ca651-127">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ca651-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ca651-128">инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="ca651-128">installStateDetail</span></span>|[<span data-ttu-id="ca651-129">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="ca651-129">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="ca651-130">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="ca651-130">The install state detail of the app.</span></span> <span data-ttu-id="ca651-131">Возможные значения:,,,,,,,,,,,,,,,,,, `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` , `seeUninstallErrorCode` , `pendingReboot` , `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` ,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="ca651-131">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="ca651-132">errorCode</span><span class="sxs-lookup"><span data-stu-id="ca651-132">errorCode</span></span>|<span data-ttu-id="ca651-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ca651-133">Int32</span></span>|<span data-ttu-id="ca651-134">Код ошибки для установки или удаления сбоев конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ca651-134">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="ca651-135">таржетластсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="ca651-135">targetLastSyncDateTime</span></span>|<span data-ttu-id="ca651-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca651-136">DateTimeOffset</span></span>|<span data-ttu-id="ca651-137">Время последней синхронизации конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ca651-137">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca651-138">Связи</span><span class="sxs-lookup"><span data-stu-id="ca651-138">Relationships</span></span>
<span data-ttu-id="ca651-139">Нет</span><span class="sxs-lookup"><span data-stu-id="ca651-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca651-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca651-140">JSON Representation</span></span>
<span data-ttu-id="ca651-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca651-141">Here is a JSON representation of the resource.</span></span>
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





