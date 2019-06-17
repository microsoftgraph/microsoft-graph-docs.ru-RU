---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6013482fe69aa7a4ccf789c677ef448e0a277991
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993356"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="50c30-103">Тип ресурса Мобилеаппрелатионшипстате</span><span class="sxs-lookup"><span data-stu-id="50c30-103">mobileAppRelationshipState resource type</span></span>

> <span data-ttu-id="50c30-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50c30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50c30-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50c30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50c30-106">Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.</span><span class="sxs-lookup"><span data-stu-id="50c30-106">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="50c30-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="50c30-107">Properties</span></span>
|<span data-ttu-id="50c30-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="50c30-108">Property</span></span>|<span data-ttu-id="50c30-109">Тип</span><span class="sxs-lookup"><span data-stu-id="50c30-109">Type</span></span>|<span data-ttu-id="50c30-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50c30-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50c30-111">Саурцеидс</span><span class="sxs-lookup"><span data-stu-id="50c30-111">sourceIds</span></span>|<span data-ttu-id="50c30-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="50c30-112">String collection</span></span>|<span data-ttu-id="50c30-113">Коллекция идентификаторов исходного приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="50c30-113">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="50c30-114">targetId</span><span class="sxs-lookup"><span data-stu-id="50c30-114">targetId</span></span>|<span data-ttu-id="50c30-115">String</span><span class="sxs-lookup"><span data-stu-id="50c30-115">String</span></span>|<span data-ttu-id="50c30-116">Идентификатор связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="50c30-116">The related target app's id.</span></span>|
|<span data-ttu-id="50c30-117">Таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="50c30-117">targetDisplayName</span></span>|<span data-ttu-id="50c30-118">String</span><span class="sxs-lookup"><span data-stu-id="50c30-118">String</span></span>|<span data-ttu-id="50c30-119">Отображаемое имя связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="50c30-119">The related target app's display name.</span></span>|
|<span data-ttu-id="50c30-120">deviceId</span><span class="sxs-lookup"><span data-stu-id="50c30-120">deviceId</span></span>|<span data-ttu-id="50c30-121">String</span><span class="sxs-lookup"><span data-stu-id="50c30-121">String</span></span>|<span data-ttu-id="50c30-122">Соответствующий идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="50c30-122">The corresponding device id.</span></span>|
|<span data-ttu-id="50c30-123">installState</span><span class="sxs-lookup"><span data-stu-id="50c30-123">installState</span></span>|[<span data-ttu-id="50c30-124">Ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="50c30-124">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="50c30-125">Состояние установки приложения конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="50c30-125">The install state of the app of target app.</span></span> <span data-ttu-id="50c30-126">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="50c30-126">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="50c30-127">Инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="50c30-127">installStateDetail</span></span>|[<span data-ttu-id="50c30-128">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="50c30-128">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="50c30-129">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="50c30-129">The install state detail of the app.</span></span> <span data-ttu-id="50c30-130">Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`,,,,,,,,,,,,,,,,,,,,, `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="50c30-130">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="50c30-131">errorCode</span><span class="sxs-lookup"><span data-stu-id="50c30-131">errorCode</span></span>|<span data-ttu-id="50c30-132">Int32</span><span class="sxs-lookup"><span data-stu-id="50c30-132">Int32</span></span>|<span data-ttu-id="50c30-133">Код ошибки для установки или удаления сбоев конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="50c30-133">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="50c30-134">Таржетластсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="50c30-134">targetLastSyncDateTime</span></span>|<span data-ttu-id="50c30-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50c30-135">DateTimeOffset</span></span>|<span data-ttu-id="50c30-136">Время последней синхронизации конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="50c30-136">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50c30-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="50c30-137">Relationships</span></span>
<span data-ttu-id="50c30-138">Нет</span><span class="sxs-lookup"><span data-stu-id="50c30-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50c30-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50c30-139">JSON Representation</span></span>
<span data-ttu-id="50c30-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50c30-140">Here is a JSON representation of the resource.</span></span>
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





