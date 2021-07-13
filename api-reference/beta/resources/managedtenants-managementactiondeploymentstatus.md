---
title: тип ресурса managementActionDeploymentStatus
description: Представляет состояние развертывания для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: efd789a7b4b48098e8d679273da1152f6611a28c
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403044"
---
# <a name="managementactiondeploymentstatus-resource-type"></a><span data-ttu-id="cd64c-103">тип ресурса managementActionDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="cd64c-103">managementActionDeploymentStatus resource type</span></span>

<span data-ttu-id="cd64c-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="cd64c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd64c-105">Представляет состояние развертывания для данного управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="cd64c-105">Represents the deployment status for a given managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="cd64c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd64c-106">Properties</span></span>
|<span data-ttu-id="cd64c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd64c-107">Property</span></span>|<span data-ttu-id="cd64c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cd64c-108">Type</span></span>|<span data-ttu-id="cd64c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cd64c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd64c-110">managementActionId</span><span class="sxs-lookup"><span data-stu-id="cd64c-110">managementActionId</span></span>|<span data-ttu-id="cd64c-111">String</span><span class="sxs-lookup"><span data-stu-id="cd64c-111">String</span></span>|<span data-ttu-id="cd64c-112">Идентификатор для действия управления.</span><span class="sxs-lookup"><span data-stu-id="cd64c-112">The identifier for the management action.</span></span> <span data-ttu-id="cd64c-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd64c-113">Required.</span></span> <span data-ttu-id="cd64c-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd64c-114">Read-only.</span></span>|
|<span data-ttu-id="cd64c-115">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="cd64c-115">managementTemplateId</span></span>|<span data-ttu-id="cd64c-116">String</span><span class="sxs-lookup"><span data-stu-id="cd64c-116">String</span></span>|<span data-ttu-id="cd64c-117">Идентификатор шаблона управления, который использовался для создания действия управления.</span><span class="sxs-lookup"><span data-stu-id="cd64c-117">The management template identifier that was used to generate the management action.</span></span> <span data-ttu-id="cd64c-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd64c-118">Required.</span></span> <span data-ttu-id="cd64c-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd64c-119">Read-only.</span></span>|
|<span data-ttu-id="cd64c-120">status</span><span class="sxs-lookup"><span data-stu-id="cd64c-120">status</span></span>|<span data-ttu-id="cd64c-121">managementActionStatus</span><span class="sxs-lookup"><span data-stu-id="cd64c-121">managementActionStatus</span></span>|<span data-ttu-id="cd64c-122">Состояние действия управления.</span><span class="sxs-lookup"><span data-stu-id="cd64c-122">The status of the management action.</span></span> <span data-ttu-id="cd64c-123">Возможные значения: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="cd64c-123">Possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`.</span></span> <span data-ttu-id="cd64c-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd64c-124">Required.</span></span>|
|<span data-ttu-id="cd64c-125">workloadActionDeploymentStatuses</span><span class="sxs-lookup"><span data-stu-id="cd64c-125">workloadActionDeploymentStatuses</span></span>|<span data-ttu-id="cd64c-126">[коллекция microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="cd64c-126">[microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md) collection</span></span>|<span data-ttu-id="cd64c-127">Коллекция статуй развертывания действий рабочей нагрузки для данного действия управления.</span><span class="sxs-lookup"><span data-stu-id="cd64c-127">The collection of workload action deployment statues for the given management action.</span></span> <span data-ttu-id="cd64c-128">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="cd64c-128">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd64c-129">Связи</span><span class="sxs-lookup"><span data-stu-id="cd64c-129">Relationships</span></span>
<span data-ttu-id="cd64c-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cd64c-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd64c-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cd64c-131">JSON representation</span></span>
<span data-ttu-id="cd64c-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd64c-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionDeploymentStatus",
  "managementTemplateId": "String",
  "managementActionId": "String",
  "status": "String",
  "workloadActionDeploymentStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
    }
  ]
}
```
