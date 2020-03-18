---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d17dfb7cc288edb37f82587dfe76b65ebe15efd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781581"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="9298a-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="9298a-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="9298a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9298a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9298a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9298a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9298a-106">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="9298a-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="9298a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9298a-107">Properties</span></span>
|<span data-ttu-id="9298a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9298a-108">Property</span></span>|<span data-ttu-id="9298a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9298a-109">Type</span></span>|<span data-ttu-id="9298a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9298a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9298a-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9298a-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="9298a-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9298a-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9298a-113">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="9298a-113">Deployment of an app.</span></span>|
|<span data-ttu-id="9298a-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="9298a-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="9298a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9298a-115">Int32</span></span>|<span data-ttu-id="9298a-116">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="9298a-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9298a-117">Связи</span><span class="sxs-lookup"><span data-stu-id="9298a-117">Relationships</span></span>
<span data-ttu-id="9298a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9298a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9298a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9298a-119">JSON Representation</span></span>
<span data-ttu-id="9298a-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9298a-120">Here is a JSON representation of the resource.</span></span>
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



