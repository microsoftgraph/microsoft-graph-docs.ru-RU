---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 211b40c397ec7e3fb4000c8f4459056edec2a6f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972203"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="b3e4b-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="b3e4b-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="b3e4b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b3e4b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3e4b-105">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="b3e4b-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="b3e4b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3e4b-106">Properties</span></span>
|<span data-ttu-id="b3e4b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3e4b-107">Property</span></span>|<span data-ttu-id="b3e4b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b3e4b-108">Type</span></span>|<span data-ttu-id="b3e4b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b3e4b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3e4b-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b3e4b-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="b3e4b-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b3e4b-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b3e4b-112">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="b3e4b-112">Deployment of an app.</span></span>|
|<span data-ttu-id="b3e4b-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="b3e4b-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="b3e4b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b3e4b-114">Int32</span></span>|<span data-ttu-id="b3e4b-115">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="b3e4b-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3e4b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="b3e4b-116">Relationships</span></span>
<span data-ttu-id="b3e4b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b3e4b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3e4b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3e4b-118">JSON Representation</span></span>
<span data-ttu-id="b3e4b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3e4b-119">Here is a JSON representation of the resource.</span></span>
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



