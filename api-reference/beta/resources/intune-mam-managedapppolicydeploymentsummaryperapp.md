---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b54021290b6cc66be6cd33c15bcda3492aca1cb0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730989"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="a67cf-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="a67cf-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="a67cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a67cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a67cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a67cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a67cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a67cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a67cf-107">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="a67cf-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="a67cf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a67cf-108">Properties</span></span>
|<span data-ttu-id="a67cf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a67cf-109">Property</span></span>|<span data-ttu-id="a67cf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a67cf-110">Type</span></span>|<span data-ttu-id="a67cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a67cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a67cf-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a67cf-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="a67cf-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a67cf-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a67cf-114">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="a67cf-114">Deployment of an app.</span></span>|
|<span data-ttu-id="a67cf-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="a67cf-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="a67cf-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a67cf-116">Int32</span></span>|<span data-ttu-id="a67cf-117">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="a67cf-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a67cf-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a67cf-118">Relationships</span></span>
<span data-ttu-id="a67cf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a67cf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a67cf-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a67cf-120">JSON Representation</span></span>
<span data-ttu-id="a67cf-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a67cf-121">Here is a JSON representation of the resource.</span></span>
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





