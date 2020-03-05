---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bf9ff99bdcbfb7ea484a656c540449161a53d45d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448363"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="5ecb1-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="5ecb1-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="5ecb1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5ecb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ecb1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ecb1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ecb1-106">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="5ecb1-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="5ecb1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ecb1-107">Properties</span></span>
|<span data-ttu-id="5ecb1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ecb1-108">Property</span></span>|<span data-ttu-id="5ecb1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5ecb1-109">Type</span></span>|<span data-ttu-id="5ecb1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5ecb1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ecb1-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5ecb1-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="5ecb1-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5ecb1-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5ecb1-113">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="5ecb1-113">Deployment of an app.</span></span>|
|<span data-ttu-id="5ecb1-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="5ecb1-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="5ecb1-115">Int32</span><span class="sxs-lookup"><span data-stu-id="5ecb1-115">Int32</span></span>|<span data-ttu-id="5ecb1-116">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="5ecb1-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ecb1-117">Связи</span><span class="sxs-lookup"><span data-stu-id="5ecb1-117">Relationships</span></span>
<span data-ttu-id="5ecb1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5ecb1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ecb1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ecb1-119">JSON Representation</span></span>
<span data-ttu-id="5ecb1-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ecb1-120">Here is a JSON representation of the resource.</span></span>
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




