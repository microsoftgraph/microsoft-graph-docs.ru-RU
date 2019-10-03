---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70c46530f979f7372b3592c310d4434246c5f0c1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367800"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="40184-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="40184-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="40184-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40184-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40184-105">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="40184-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="40184-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="40184-106">Properties</span></span>
|<span data-ttu-id="40184-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="40184-107">Property</span></span>|<span data-ttu-id="40184-108">Тип</span><span class="sxs-lookup"><span data-stu-id="40184-108">Type</span></span>|<span data-ttu-id="40184-109">Описание</span><span class="sxs-lookup"><span data-stu-id="40184-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40184-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="40184-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="40184-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="40184-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="40184-112">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="40184-112">Deployment of an app.</span></span>|
|<span data-ttu-id="40184-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="40184-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="40184-114">Int32</span><span class="sxs-lookup"><span data-stu-id="40184-114">Int32</span></span>|<span data-ttu-id="40184-115">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="40184-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40184-116">Связи</span><span class="sxs-lookup"><span data-stu-id="40184-116">Relationships</span></span>
<span data-ttu-id="40184-117">Нет</span><span class="sxs-lookup"><span data-stu-id="40184-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40184-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40184-118">JSON Representation</span></span>
<span data-ttu-id="40184-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40184-119">Here is a JSON representation of the resource.</span></span>
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




