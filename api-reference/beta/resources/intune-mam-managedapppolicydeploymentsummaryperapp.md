---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac5acf2536b669c42a324fd5761bed6333dbf05a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932961"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="36373-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="36373-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="36373-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="36373-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36373-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36373-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36373-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36373-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36373-107">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="36373-107">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="36373-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="36373-108">Properties</span></span>
|<span data-ttu-id="36373-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="36373-109">Property</span></span>|<span data-ttu-id="36373-110">Тип</span><span class="sxs-lookup"><span data-stu-id="36373-110">Type</span></span>|<span data-ttu-id="36373-111">Описание</span><span class="sxs-lookup"><span data-stu-id="36373-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36373-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="36373-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="36373-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="36373-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="36373-114">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="36373-114">Deployment of an app.</span></span>|
|<span data-ttu-id="36373-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="36373-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="36373-116">Int32</span><span class="sxs-lookup"><span data-stu-id="36373-116">Int32</span></span>|<span data-ttu-id="36373-117">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="36373-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36373-118">Связи</span><span class="sxs-lookup"><span data-stu-id="36373-118">Relationships</span></span>
<span data-ttu-id="36373-119">Нет</span><span class="sxs-lookup"><span data-stu-id="36373-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="36373-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36373-120">JSON Representation</span></span>
<span data-ttu-id="36373-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36373-121">Here is a JSON representation of the resource.</span></span>
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





