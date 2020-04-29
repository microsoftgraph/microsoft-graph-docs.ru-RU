---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a0a4189c1f26736231155da775f137e7f61bbd23
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468495"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="f963c-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="f963c-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="f963c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f963c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f963c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f963c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f963c-106">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="f963c-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="f963c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f963c-107">Properties</span></span>
|<span data-ttu-id="f963c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f963c-108">Property</span></span>|<span data-ttu-id="f963c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f963c-109">Type</span></span>|<span data-ttu-id="f963c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f963c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f963c-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f963c-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="f963c-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f963c-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f963c-113">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="f963c-113">Deployment of an app.</span></span>|
|<span data-ttu-id="f963c-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="f963c-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="f963c-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f963c-115">Int32</span></span>|<span data-ttu-id="f963c-116">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="f963c-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f963c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f963c-117">Relationships</span></span>
<span data-ttu-id="f963c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f963c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f963c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f963c-119">JSON Representation</span></span>
<span data-ttu-id="f963c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f963c-120">Here is a JSON representation of the resource.</span></span>
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







