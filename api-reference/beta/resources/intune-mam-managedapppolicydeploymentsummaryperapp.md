---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5802d8f1d29174a8e4e01ee10e4bf66081d12ca6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373079"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="88627-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="88627-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="88627-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88627-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88627-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88627-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88627-106">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="88627-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="88627-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="88627-107">Properties</span></span>
|<span data-ttu-id="88627-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="88627-108">Property</span></span>|<span data-ttu-id="88627-109">Тип</span><span class="sxs-lookup"><span data-stu-id="88627-109">Type</span></span>|<span data-ttu-id="88627-110">Описание</span><span class="sxs-lookup"><span data-stu-id="88627-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88627-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="88627-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="88627-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="88627-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="88627-113">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="88627-113">Deployment of an app.</span></span>|
|<span data-ttu-id="88627-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="88627-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="88627-115">Int32</span><span class="sxs-lookup"><span data-stu-id="88627-115">Int32</span></span>|<span data-ttu-id="88627-116">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="88627-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88627-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="88627-117">Relationships</span></span>
<span data-ttu-id="88627-118">Нет</span><span class="sxs-lookup"><span data-stu-id="88627-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88627-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88627-119">JSON Representation</span></span>
<span data-ttu-id="88627-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88627-120">Here is a JSON representation of the resource.</span></span>
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



