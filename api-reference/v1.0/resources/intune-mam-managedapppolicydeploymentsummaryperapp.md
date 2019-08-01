---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84befe8b98b2e0e6883328c09bdee16e2720300d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037942"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="c1a9e-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="c1a9e-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="c1a9e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1a9e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1a9e-105">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="c1a9e-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="c1a9e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1a9e-106">Properties</span></span>
|<span data-ttu-id="c1a9e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1a9e-107">Property</span></span>|<span data-ttu-id="c1a9e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c1a9e-108">Type</span></span>|<span data-ttu-id="c1a9e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c1a9e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a9e-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c1a9e-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="c1a9e-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c1a9e-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c1a9e-112">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="c1a9e-112">Deployment of an app.</span></span>|
|<span data-ttu-id="c1a9e-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="c1a9e-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="c1a9e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c1a9e-114">Int32</span></span>|<span data-ttu-id="c1a9e-115">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="c1a9e-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1a9e-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1a9e-116">Relationships</span></span>
<span data-ttu-id="c1a9e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c1a9e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1a9e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1a9e-118">JSON Representation</span></span>
<span data-ttu-id="c1a9e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1a9e-119">Here is a JSON representation of the resource.</span></span>
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



