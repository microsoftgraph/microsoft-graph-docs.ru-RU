---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 149a578f60ba5953f77c83ca2fbc3810931dffff
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262512"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="a651b-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="a651b-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="a651b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a651b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a651b-105">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="a651b-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="a651b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a651b-106">Properties</span></span>
|<span data-ttu-id="a651b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a651b-107">Property</span></span>|<span data-ttu-id="a651b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a651b-108">Type</span></span>|<span data-ttu-id="a651b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a651b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a651b-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a651b-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="a651b-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a651b-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a651b-112">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="a651b-112">Deployment of an app.</span></span>|
|<span data-ttu-id="a651b-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="a651b-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="a651b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a651b-114">Int32</span></span>|<span data-ttu-id="a651b-115">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="a651b-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a651b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a651b-116">Relationships</span></span>
<span data-ttu-id="a651b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a651b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a651b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a651b-118">JSON Representation</span></span>
<span data-ttu-id="a651b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a651b-119">Here is a JSON representation of the resource.</span></span>
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



