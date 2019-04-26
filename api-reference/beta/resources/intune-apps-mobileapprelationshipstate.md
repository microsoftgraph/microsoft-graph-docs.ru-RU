---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7f3dcbbc2544a4231cd5da102985d7142feb03a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551801"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="dfbed-103">Тип ресурса Мобилеаппрелатионшипстате</span><span class="sxs-lookup"><span data-stu-id="dfbed-103">mobileAppRelationshipState resource type</span></span>

> <span data-ttu-id="dfbed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfbed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfbed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfbed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfbed-106">Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.</span><span class="sxs-lookup"><span data-stu-id="dfbed-106">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="dfbed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfbed-107">Properties</span></span>
|<span data-ttu-id="dfbed-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfbed-108">Property</span></span>|<span data-ttu-id="dfbed-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dfbed-109">Type</span></span>|<span data-ttu-id="dfbed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dfbed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfbed-111">Саурцеидс</span><span class="sxs-lookup"><span data-stu-id="dfbed-111">sourceIds</span></span>|<span data-ttu-id="dfbed-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dfbed-112">String collection</span></span>|<span data-ttu-id="dfbed-113">Коллекция идентификаторов исходного приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="dfbed-113">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="dfbed-114">targetId</span><span class="sxs-lookup"><span data-stu-id="dfbed-114">targetId</span></span>|<span data-ttu-id="dfbed-115">String</span><span class="sxs-lookup"><span data-stu-id="dfbed-115">String</span></span>|<span data-ttu-id="dfbed-116">Идентификатор связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="dfbed-116">The related target app's id.</span></span>|
|<span data-ttu-id="dfbed-117">Таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="dfbed-117">targetDisplayName</span></span>|<span data-ttu-id="dfbed-118">String</span><span class="sxs-lookup"><span data-stu-id="dfbed-118">String</span></span>|<span data-ttu-id="dfbed-119">Отображаемое имя связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="dfbed-119">The related target app's display name.</span></span>|
|<span data-ttu-id="dfbed-120">deviceId</span><span class="sxs-lookup"><span data-stu-id="dfbed-120">deviceId</span></span>|<span data-ttu-id="dfbed-121">String</span><span class="sxs-lookup"><span data-stu-id="dfbed-121">String</span></span>|<span data-ttu-id="dfbed-122">Соответствующий идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="dfbed-122">The corresponding device id.</span></span>|
|<span data-ttu-id="dfbed-123">installState</span><span class="sxs-lookup"><span data-stu-id="dfbed-123">installState</span></span>|[<span data-ttu-id="dfbed-124">Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="dfbed-124">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="dfbed-125">Состояние установки приложения конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="dfbed-125">The install state of the app of target app.</span></span> <span data-ttu-id="dfbed-126">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="dfbed-126">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="dfbed-127">Инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="dfbed-127">installStateDetail</span></span>|[<span data-ttu-id="dfbed-128">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="dfbed-128">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="dfbed-129">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="dfbed-129">The install state detail of the app.</span></span> <span data-ttu-id="dfbed-130">Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`,,,,,,,,,,,,,,,,,,,,, `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="dfbed-130">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="dfbed-131">errorCode</span><span class="sxs-lookup"><span data-stu-id="dfbed-131">errorCode</span></span>|<span data-ttu-id="dfbed-132">Int32</span><span class="sxs-lookup"><span data-stu-id="dfbed-132">Int32</span></span>|<span data-ttu-id="dfbed-133">Код ошибки для установки или удаления сбоев конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="dfbed-133">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="dfbed-134">Таржетластсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="dfbed-134">targetLastSyncDateTime</span></span>|<span data-ttu-id="dfbed-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfbed-135">DateTimeOffset</span></span>|<span data-ttu-id="dfbed-136">Время последней синхронизации конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="dfbed-136">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfbed-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="dfbed-137">Relationships</span></span>
<span data-ttu-id="dfbed-138">Нет</span><span class="sxs-lookup"><span data-stu-id="dfbed-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfbed-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfbed-139">JSON Representation</span></span>
<span data-ttu-id="dfbed-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfbed-140">Here is a JSON representation of the resource.</span></span>
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





