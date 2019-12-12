---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eef4e5788be1c725ce9bfe2bc6fb2bd298394450
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955738"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="db18d-103">Тип ресурса Мобилеаппрелатионшипстате</span><span class="sxs-lookup"><span data-stu-id="db18d-103">mobileAppRelationshipState resource type</span></span>

> <span data-ttu-id="db18d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db18d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db18d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db18d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db18d-106">Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.</span><span class="sxs-lookup"><span data-stu-id="db18d-106">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="db18d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="db18d-107">Properties</span></span>
|<span data-ttu-id="db18d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="db18d-108">Property</span></span>|<span data-ttu-id="db18d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="db18d-109">Type</span></span>|<span data-ttu-id="db18d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db18d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db18d-111">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="db18d-111">sourceIds</span></span>|<span data-ttu-id="db18d-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="db18d-112">String collection</span></span>|<span data-ttu-id="db18d-113">Коллекция идентификаторов исходного приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="db18d-113">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="db18d-114">targetId</span><span class="sxs-lookup"><span data-stu-id="db18d-114">targetId</span></span>|<span data-ttu-id="db18d-115">Строка</span><span class="sxs-lookup"><span data-stu-id="db18d-115">String</span></span>|<span data-ttu-id="db18d-116">Идентификатор связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="db18d-116">The related target app's id.</span></span>|
|<span data-ttu-id="db18d-117">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="db18d-117">targetDisplayName</span></span>|<span data-ttu-id="db18d-118">Строка</span><span class="sxs-lookup"><span data-stu-id="db18d-118">String</span></span>|<span data-ttu-id="db18d-119">Отображаемое имя связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="db18d-119">The related target app's display name.</span></span>|
|<span data-ttu-id="db18d-120">deviceId</span><span class="sxs-lookup"><span data-stu-id="db18d-120">deviceId</span></span>|<span data-ttu-id="db18d-121">String</span><span class="sxs-lookup"><span data-stu-id="db18d-121">String</span></span>|<span data-ttu-id="db18d-122">Соответствующий идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="db18d-122">The corresponding device id.</span></span>|
|<span data-ttu-id="db18d-123">installState</span><span class="sxs-lookup"><span data-stu-id="db18d-123">installState</span></span>|[<span data-ttu-id="db18d-124">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="db18d-124">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="db18d-125">Состояние установки приложения конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="db18d-125">The install state of the app of target app.</span></span> <span data-ttu-id="db18d-126">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="db18d-126">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="db18d-127">инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="db18d-127">installStateDetail</span></span>|[<span data-ttu-id="db18d-128">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="db18d-128">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="db18d-129">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="db18d-129">The install state detail of the app.</span></span> <span data-ttu-id="db18d-130">Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="db18d-130">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="db18d-131">errorCode</span><span class="sxs-lookup"><span data-stu-id="db18d-131">errorCode</span></span>|<span data-ttu-id="db18d-132">Int32</span><span class="sxs-lookup"><span data-stu-id="db18d-132">Int32</span></span>|<span data-ttu-id="db18d-133">Код ошибки для установки или удаления сбоев конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="db18d-133">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="db18d-134">таржетластсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="db18d-134">targetLastSyncDateTime</span></span>|<span data-ttu-id="db18d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db18d-135">DateTimeOffset</span></span>|<span data-ttu-id="db18d-136">Время последней синхронизации конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="db18d-136">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db18d-137">Связи</span><span class="sxs-lookup"><span data-stu-id="db18d-137">Relationships</span></span>
<span data-ttu-id="db18d-138">Нет</span><span class="sxs-lookup"><span data-stu-id="db18d-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db18d-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db18d-139">JSON Representation</span></span>
<span data-ttu-id="db18d-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db18d-140">Here is a JSON representation of the resource.</span></span>
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



