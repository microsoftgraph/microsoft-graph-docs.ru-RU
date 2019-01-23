---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0e6053a1d690a68359fa30d5e5ac4c0ce5520bc6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411094"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="ed675-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="ed675-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="ed675-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed675-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ed675-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed675-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed675-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed675-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed675-107">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="ed675-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="ed675-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed675-108">Properties</span></span>
|<span data-ttu-id="ed675-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed675-109">Property</span></span>|<span data-ttu-id="ed675-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ed675-110">Type</span></span>|<span data-ttu-id="ed675-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed675-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed675-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed675-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="ed675-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed675-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ed675-114">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="ed675-114">Deployment of an app.</span></span>|
|<span data-ttu-id="ed675-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="ed675-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="ed675-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ed675-116">Int32</span></span>|<span data-ttu-id="ed675-117">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="ed675-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed675-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ed675-118">Relationships</span></span>
<span data-ttu-id="ed675-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ed675-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed675-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed675-120">JSON Representation</span></span>
<span data-ttu-id="ed675-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed675-121">Here is a JSON representation of the resource.</span></span>
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




