---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 23966e2017780d3dcfde592d7159576403fe3192
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829752"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="ea273-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="ea273-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="ea273-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea273-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea273-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea273-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea273-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea273-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea273-107">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="ea273-107">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="ea273-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea273-108">Properties</span></span>
|<span data-ttu-id="ea273-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea273-109">Property</span></span>|<span data-ttu-id="ea273-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea273-110">Type</span></span>|<span data-ttu-id="ea273-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea273-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea273-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ea273-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="ea273-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ea273-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ea273-114">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="ea273-114">Deployment of an app.</span></span>|
|<span data-ttu-id="ea273-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="ea273-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="ea273-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ea273-116">Int32</span></span>|<span data-ttu-id="ea273-117">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="ea273-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea273-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ea273-118">Relationships</span></span>
<span data-ttu-id="ea273-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ea273-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea273-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea273-120">JSON Representation</span></span>
<span data-ttu-id="ea273-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea273-121">Here is a JSON representation of the resource.</span></span>
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





