---
title: Тип ресурса managedAppPolicyDeploymentSummaryPerApp
description: Представляет сводку по развертыванию политик для приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7082c3f3b1bd4d52970f2af223c55770c686be0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041296"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="1b330-103">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="1b330-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

<span data-ttu-id="1b330-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b330-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b330-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b330-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b330-106">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="1b330-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="1b330-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b330-107">Properties</span></span>
|<span data-ttu-id="1b330-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b330-108">Property</span></span>|<span data-ttu-id="1b330-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1b330-109">Type</span></span>|<span data-ttu-id="1b330-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1b330-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b330-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1b330-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="1b330-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1b330-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="1b330-113">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="1b330-113">Deployment of an app.</span></span>|
|<span data-ttu-id="1b330-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="1b330-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="1b330-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1b330-115">Int32</span></span>|<span data-ttu-id="1b330-116">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="1b330-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b330-117">Связи</span><span class="sxs-lookup"><span data-stu-id="1b330-117">Relationships</span></span>
<span data-ttu-id="1b330-118">Нет</span><span class="sxs-lookup"><span data-stu-id="1b330-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b330-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b330-119">JSON Representation</span></span>
<span data-ttu-id="1b330-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b330-120">Here is a JSON representation of the resource.</span></span>
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









