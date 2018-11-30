---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
ms.openlocfilehash: 56b7952049c6ad41ee46f6b77c821aa32b1c4de8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027364"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="51ff9-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="51ff9-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="51ff9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51ff9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51ff9-105">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="51ff9-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="51ff9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="51ff9-106">Properties</span></span>
|<span data-ttu-id="51ff9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="51ff9-107">Property</span></span>|<span data-ttu-id="51ff9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="51ff9-108">Type</span></span>|<span data-ttu-id="51ff9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51ff9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ff9-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="51ff9-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="51ff9-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="51ff9-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="51ff9-112">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="51ff9-112">Deployment of an app.</span></span>|
|<span data-ttu-id="51ff9-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="51ff9-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="51ff9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="51ff9-114">Int32</span></span>|<span data-ttu-id="51ff9-115">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="51ff9-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51ff9-116">Связи</span><span class="sxs-lookup"><span data-stu-id="51ff9-116">Relationships</span></span>
<span data-ttu-id="51ff9-117">Нет</span><span class="sxs-lookup"><span data-stu-id="51ff9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51ff9-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51ff9-118">JSON Representation</span></span>
<span data-ttu-id="51ff9-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51ff9-119">Here is a JSON representation of the resource.</span></span>
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



