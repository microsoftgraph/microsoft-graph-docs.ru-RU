---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1bcf69e4a8d24af3f0ada2ceae5730cc0cfdc18
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752331"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="55953-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="55953-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="55953-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55953-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55953-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55953-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55953-106">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="55953-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="55953-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="55953-107">Properties</span></span>
|<span data-ttu-id="55953-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="55953-108">Property</span></span>|<span data-ttu-id="55953-109">Тип</span><span class="sxs-lookup"><span data-stu-id="55953-109">Type</span></span>|<span data-ttu-id="55953-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55953-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55953-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="55953-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="55953-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="55953-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="55953-113">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="55953-113">Deployment of an app.</span></span>|
|<span data-ttu-id="55953-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="55953-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="55953-115">Int32</span><span class="sxs-lookup"><span data-stu-id="55953-115">Int32</span></span>|<span data-ttu-id="55953-116">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="55953-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55953-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="55953-117">Relationships</span></span>
<span data-ttu-id="55953-118">Нет</span><span class="sxs-lookup"><span data-stu-id="55953-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55953-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55953-119">JSON Representation</span></span>
<span data-ttu-id="55953-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55953-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "configurationAppliedUserCount": 1024
}
```




