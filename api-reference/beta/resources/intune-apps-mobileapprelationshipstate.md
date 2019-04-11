---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7f3dcbbc2544a4231cd5da102985d7142feb03a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809310"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="ee95f-103">Тип ресурса Мобилеаппрелатионшипстате</span><span class="sxs-lookup"><span data-stu-id="ee95f-103">mobileAppRelationshipState resource type</span></span>

> <span data-ttu-id="ee95f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee95f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee95f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee95f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee95f-106">Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.</span><span class="sxs-lookup"><span data-stu-id="ee95f-106">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="ee95f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee95f-107">Properties</span></span>
|<span data-ttu-id="ee95f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee95f-108">Property</span></span>|<span data-ttu-id="ee95f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ee95f-109">Type</span></span>|<span data-ttu-id="ee95f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ee95f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee95f-111">Саурцеидс</span><span class="sxs-lookup"><span data-stu-id="ee95f-111">sourceIds</span></span>|<span data-ttu-id="ee95f-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ee95f-112">String collection</span></span>|<span data-ttu-id="ee95f-113">Коллекция идентификаторов исходного приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="ee95f-113">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="ee95f-114">targetId</span><span class="sxs-lookup"><span data-stu-id="ee95f-114">targetId</span></span>|<span data-ttu-id="ee95f-115">String</span><span class="sxs-lookup"><span data-stu-id="ee95f-115">String</span></span>|<span data-ttu-id="ee95f-116">Идентификатор связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ee95f-116">The related target app's id.</span></span>|
|<span data-ttu-id="ee95f-117">Таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="ee95f-117">targetDisplayName</span></span>|<span data-ttu-id="ee95f-118">String</span><span class="sxs-lookup"><span data-stu-id="ee95f-118">String</span></span>|<span data-ttu-id="ee95f-119">Отображаемое имя связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ee95f-119">The related target app's display name.</span></span>|
|<span data-ttu-id="ee95f-120">deviceId</span><span class="sxs-lookup"><span data-stu-id="ee95f-120">deviceId</span></span>|<span data-ttu-id="ee95f-121">String</span><span class="sxs-lookup"><span data-stu-id="ee95f-121">String</span></span>|<span data-ttu-id="ee95f-122">Соответствующий идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="ee95f-122">The corresponding device id.</span></span>|
|<span data-ttu-id="ee95f-123">installState</span><span class="sxs-lookup"><span data-stu-id="ee95f-123">installState</span></span>|[<span data-ttu-id="ee95f-124">Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="ee95f-124">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ee95f-125">Состояние установки приложения конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ee95f-125">The install state of the app of target app.</span></span> <span data-ttu-id="ee95f-126">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ee95f-126">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ee95f-127">Инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="ee95f-127">installStateDetail</span></span>|[<span data-ttu-id="ee95f-128">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="ee95f-128">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="ee95f-129">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="ee95f-129">The install state detail of the app.</span></span> <span data-ttu-id="ee95f-130">Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`,,,,,,,,,,,,,,,,,,,,, `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ee95f-130">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="ee95f-131">errorCode</span><span class="sxs-lookup"><span data-stu-id="ee95f-131">errorCode</span></span>|<span data-ttu-id="ee95f-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ee95f-132">Int32</span></span>|<span data-ttu-id="ee95f-133">Код ошибки для установки или удаления сбоев конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ee95f-133">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="ee95f-134">Таржетластсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="ee95f-134">targetLastSyncDateTime</span></span>|<span data-ttu-id="ee95f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee95f-135">DateTimeOffset</span></span>|<span data-ttu-id="ee95f-136">Время последней синхронизации конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="ee95f-136">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee95f-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="ee95f-137">Relationships</span></span>
<span data-ttu-id="ee95f-138">Нет</span><span class="sxs-lookup"><span data-stu-id="ee95f-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee95f-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee95f-139">JSON Representation</span></span>
<span data-ttu-id="ee95f-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee95f-140">Here is a JSON representation of the resource.</span></span>
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





