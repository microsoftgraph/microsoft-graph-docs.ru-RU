---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
ms.openlocfilehash: 2555fd72bb5b7b3e4018d99a7ddbdd6627b2cef3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079640"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="fd8b8-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="fd8b8-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="fd8b8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd8b8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd8b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd8b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd8b8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fd8b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd8b8-107">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="fd8b8-107">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="fd8b8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd8b8-108">Properties</span></span>
|<span data-ttu-id="fd8b8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd8b8-109">Property</span></span>|<span data-ttu-id="fd8b8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fd8b8-110">Type</span></span>|<span data-ttu-id="fd8b8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fd8b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd8b8-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd8b8-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="fd8b8-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd8b8-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="fd8b8-114">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="fd8b8-114">Deployment of an app.</span></span>|
|<span data-ttu-id="fd8b8-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="fd8b8-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="fd8b8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fd8b8-116">Int32</span></span>|<span data-ttu-id="fd8b8-117">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="fd8b8-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd8b8-118">Связи</span><span class="sxs-lookup"><span data-stu-id="fd8b8-118">Relationships</span></span>
<span data-ttu-id="fd8b8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="fd8b8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fd8b8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd8b8-120">JSON Representation</span></span>
<span data-ttu-id="fd8b8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd8b8-121">Here is a JSON representation of the resource.</span></span>
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





