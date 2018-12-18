---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: tfitzmac
ms.openlocfilehash: 95c05696f6c080f90b9de61c309a577924e599b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354343"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="84da2-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="84da2-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="84da2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84da2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84da2-105">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="84da2-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="84da2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="84da2-106">Properties</span></span>
|<span data-ttu-id="84da2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="84da2-107">Property</span></span>|<span data-ttu-id="84da2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="84da2-108">Type</span></span>|<span data-ttu-id="84da2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="84da2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84da2-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="84da2-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="84da2-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="84da2-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="84da2-112">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="84da2-112">Deployment of an app.</span></span>|
|<span data-ttu-id="84da2-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="84da2-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="84da2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="84da2-114">Int32</span></span>|<span data-ttu-id="84da2-115">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="84da2-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84da2-116">Связи</span><span class="sxs-lookup"><span data-stu-id="84da2-116">Relationships</span></span>
<span data-ttu-id="84da2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="84da2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84da2-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84da2-118">JSON Representation</span></span>
<span data-ttu-id="84da2-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84da2-119">Here is a JSON representation of the resource.</span></span>
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



