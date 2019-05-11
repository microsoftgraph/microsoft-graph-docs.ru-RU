---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f051c36a7d14a75b6a85a9352a6188756d0545ad
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940717"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="8c640-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="8c640-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="8c640-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c640-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c640-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c640-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c640-106">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="8c640-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="8c640-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c640-107">Properties</span></span>
|<span data-ttu-id="8c640-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c640-108">Property</span></span>|<span data-ttu-id="8c640-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8c640-109">Type</span></span>|<span data-ttu-id="8c640-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c640-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c640-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8c640-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="8c640-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8c640-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="8c640-113">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="8c640-113">Deployment of an app.</span></span>|
|<span data-ttu-id="8c640-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="8c640-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="8c640-115">Int32</span><span class="sxs-lookup"><span data-stu-id="8c640-115">Int32</span></span>|<span data-ttu-id="8c640-116">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="8c640-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c640-117">Связи</span><span class="sxs-lookup"><span data-stu-id="8c640-117">Relationships</span></span>
<span data-ttu-id="8c640-118">Нет</span><span class="sxs-lookup"><span data-stu-id="8c640-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c640-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c640-119">JSON Representation</span></span>
<span data-ttu-id="8c640-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c640-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```




