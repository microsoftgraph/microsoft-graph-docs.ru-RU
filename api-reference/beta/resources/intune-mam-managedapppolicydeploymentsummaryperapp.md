---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c95f928351be99a591e91d690a7aa9a26e556955
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161483"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="03957-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="03957-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="03957-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03957-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03957-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03957-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03957-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03957-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03957-107">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="03957-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="03957-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="03957-108">Properties</span></span>
|<span data-ttu-id="03957-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="03957-109">Property</span></span>|<span data-ttu-id="03957-110">Тип</span><span class="sxs-lookup"><span data-stu-id="03957-110">Type</span></span>|<span data-ttu-id="03957-111">Описание</span><span class="sxs-lookup"><span data-stu-id="03957-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03957-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="03957-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="03957-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="03957-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="03957-114">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="03957-114">Deployment of an app.</span></span>|
|<span data-ttu-id="03957-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="03957-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="03957-116">Int32</span><span class="sxs-lookup"><span data-stu-id="03957-116">Int32</span></span>|<span data-ttu-id="03957-117">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="03957-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03957-118">Связи</span><span class="sxs-lookup"><span data-stu-id="03957-118">Relationships</span></span>
<span data-ttu-id="03957-119">Нет</span><span class="sxs-lookup"><span data-stu-id="03957-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03957-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03957-120">JSON Representation</span></span>
<span data-ttu-id="03957-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03957-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "String"
  },
  "configurationAppliedUserCount": 1024
}
```




