---
title: Тип ресурса Мобилеаппрелатионшипстате
description: Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b76572f56e219a08a7dc7452e184e31be121ae4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491346"
---
# <a name="mobileapprelationshipstate-resource-type"></a><span data-ttu-id="eda18-103">Тип ресурса Мобилеаппрелатионшипстате</span><span class="sxs-lookup"><span data-stu-id="eda18-103">mobileAppRelationshipState resource type</span></span>

<span data-ttu-id="eda18-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eda18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eda18-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eda18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eda18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eda18-107">Описывает сведения о состоянии установки дочернего приложения в контексте имени участника-пользователя и идентификатора устройства.</span><span class="sxs-lookup"><span data-stu-id="eda18-107">Describes the installation status details of the child app in the context of UPN and device id.</span></span>

## <a name="properties"></a><span data-ttu-id="eda18-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eda18-108">Properties</span></span>
|<span data-ttu-id="eda18-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eda18-109">Property</span></span>|<span data-ttu-id="eda18-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eda18-110">Type</span></span>|<span data-ttu-id="eda18-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eda18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda18-112">саурцеидс</span><span class="sxs-lookup"><span data-stu-id="eda18-112">sourceIds</span></span>|<span data-ttu-id="eda18-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eda18-113">String collection</span></span>|<span data-ttu-id="eda18-114">Коллекция идентификаторов исходного приложения для мобильных устройств.</span><span class="sxs-lookup"><span data-stu-id="eda18-114">The collection of source mobile app's ids.</span></span>|
|<span data-ttu-id="eda18-115">targetId</span><span class="sxs-lookup"><span data-stu-id="eda18-115">targetId</span></span>|<span data-ttu-id="eda18-116">String</span><span class="sxs-lookup"><span data-stu-id="eda18-116">String</span></span>|<span data-ttu-id="eda18-117">Идентификатор связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="eda18-117">The related target app's id.</span></span>|
|<span data-ttu-id="eda18-118">таржетдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="eda18-118">targetDisplayName</span></span>|<span data-ttu-id="eda18-119">String</span><span class="sxs-lookup"><span data-stu-id="eda18-119">String</span></span>|<span data-ttu-id="eda18-120">Отображаемое имя связанного конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="eda18-120">The related target app's display name.</span></span>|
|<span data-ttu-id="eda18-121">deviceId</span><span class="sxs-lookup"><span data-stu-id="eda18-121">deviceId</span></span>|<span data-ttu-id="eda18-122">String</span><span class="sxs-lookup"><span data-stu-id="eda18-122">String</span></span>|<span data-ttu-id="eda18-123">Соответствующий идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="eda18-123">The corresponding device id.</span></span>|
|<span data-ttu-id="eda18-124">installState</span><span class="sxs-lookup"><span data-stu-id="eda18-124">installState</span></span>|[<span data-ttu-id="eda18-125">ресултантаппстате</span><span class="sxs-lookup"><span data-stu-id="eda18-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="eda18-126">Состояние установки приложения конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="eda18-126">The install state of the app of target app.</span></span> <span data-ttu-id="eda18-127">Возможные значения: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="eda18-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="eda18-128">инсталлстатедетаил</span><span class="sxs-lookup"><span data-stu-id="eda18-128">installStateDetail</span></span>|[<span data-ttu-id="eda18-129">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="eda18-129">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="eda18-130">Сведения о состоянии установки приложения.</span><span class="sxs-lookup"><span data-stu-id="eda18-130">The install state detail of the app.</span></span> <span data-ttu-id="eda18-131">Возможные значения: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="eda18-131">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="eda18-132">errorCode</span><span class="sxs-lookup"><span data-stu-id="eda18-132">errorCode</span></span>|<span data-ttu-id="eda18-133">Int32</span><span class="sxs-lookup"><span data-stu-id="eda18-133">Int32</span></span>|<span data-ttu-id="eda18-134">Код ошибки для установки или удаления сбоев конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="eda18-134">The error code for install or uninstall failures of target app.</span></span>|
|<span data-ttu-id="eda18-135">таржетластсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="eda18-135">targetLastSyncDateTime</span></span>|<span data-ttu-id="eda18-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda18-136">DateTimeOffset</span></span>|<span data-ttu-id="eda18-137">Время последней синхронизации конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="eda18-137">The last sync time of the target app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eda18-138">Связи</span><span class="sxs-lookup"><span data-stu-id="eda18-138">Relationships</span></span>
<span data-ttu-id="eda18-139">Нет</span><span class="sxs-lookup"><span data-stu-id="eda18-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eda18-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eda18-140">JSON Representation</span></span>
<span data-ttu-id="eda18-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eda18-141">Here is a JSON representation of the resource.</span></span>
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



