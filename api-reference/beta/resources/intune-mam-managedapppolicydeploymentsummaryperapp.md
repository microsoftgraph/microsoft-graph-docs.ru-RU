---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8143ce4a88fa40361c2a9c8091532172408b094c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302463"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="503bf-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="503bf-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="503bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="503bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="503bf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="503bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="503bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="503bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="503bf-107">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="503bf-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="503bf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="503bf-108">Properties</span></span>
|<span data-ttu-id="503bf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="503bf-109">Property</span></span>|<span data-ttu-id="503bf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="503bf-110">Type</span></span>|<span data-ttu-id="503bf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="503bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="503bf-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="503bf-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="503bf-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="503bf-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="503bf-114">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="503bf-114">Deployment of an app.</span></span>|
|<span data-ttu-id="503bf-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="503bf-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="503bf-116">Int32</span><span class="sxs-lookup"><span data-stu-id="503bf-116">Int32</span></span>|<span data-ttu-id="503bf-117">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="503bf-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="503bf-118">Связи</span><span class="sxs-lookup"><span data-stu-id="503bf-118">Relationships</span></span>
<span data-ttu-id="503bf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="503bf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="503bf-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="503bf-120">JSON Representation</span></span>
<span data-ttu-id="503bf-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="503bf-121">Here is a JSON representation of the resource.</span></span>
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




