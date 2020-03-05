---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 455eb414553e5bd70d1b51292b713320b09e5570
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524317"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="ab73e-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="ab73e-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="ab73e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab73e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab73e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab73e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab73e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab73e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab73e-107">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="ab73e-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="ab73e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab73e-108">Properties</span></span>
|<span data-ttu-id="ab73e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab73e-109">Property</span></span>|<span data-ttu-id="ab73e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ab73e-110">Type</span></span>|<span data-ttu-id="ab73e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab73e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab73e-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ab73e-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="ab73e-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ab73e-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ab73e-114">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="ab73e-114">Deployment of an app.</span></span>|
|<span data-ttu-id="ab73e-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="ab73e-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="ab73e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ab73e-116">Int32</span></span>|<span data-ttu-id="ab73e-117">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="ab73e-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab73e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ab73e-118">Relationships</span></span>
<span data-ttu-id="ab73e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ab73e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab73e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab73e-120">JSON Representation</span></span>
<span data-ttu-id="ab73e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab73e-121">Here is a JSON representation of the resource.</span></span>
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



