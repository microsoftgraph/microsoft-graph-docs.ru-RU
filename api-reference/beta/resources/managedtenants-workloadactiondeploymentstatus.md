---
title: workloadActionDeploymentStatus resource type
description: Представляет состояние развертывания для действия рабочей нагрузки.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a8c14b821ceabf8c8196a25c141ad8730f7151d6
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402603"
---
# <a name="workloadactiondeploymentstatus-resource-type"></a><span data-ttu-id="11846-103">workloadActionDeploymentStatus resource type</span><span class="sxs-lookup"><span data-stu-id="11846-103">workloadActionDeploymentStatus resource type</span></span>

<span data-ttu-id="11846-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="11846-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11846-105">Представляет состояние развертывания для действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="11846-105">Represents the deployment status for the workload action.</span></span>

## <a name="properties"></a><span data-ttu-id="11846-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="11846-106">Properties</span></span>
|<span data-ttu-id="11846-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="11846-107">Property</span></span>|<span data-ttu-id="11846-108">Тип</span><span class="sxs-lookup"><span data-stu-id="11846-108">Type</span></span>|<span data-ttu-id="11846-109">Описание</span><span class="sxs-lookup"><span data-stu-id="11846-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11846-110">actionId</span><span class="sxs-lookup"><span data-stu-id="11846-110">actionId</span></span>|<span data-ttu-id="11846-111">String</span><span class="sxs-lookup"><span data-stu-id="11846-111">String</span></span>|<span data-ttu-id="11846-112">Уникальный идентификатор для действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="11846-112">The unique identifier for the workload action.</span></span> <span data-ttu-id="11846-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11846-113">Required.</span></span> <span data-ttu-id="11846-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11846-114">Read-only.</span></span>|
|<span data-ttu-id="11846-115">deployedPolicyId</span><span class="sxs-lookup"><span data-stu-id="11846-115">deployedPolicyId</span></span>|<span data-ttu-id="11846-116">String</span><span class="sxs-lookup"><span data-stu-id="11846-116">String</span></span>|<span data-ttu-id="11846-117">Идентификатор любой политики, созданной с помощью действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="11846-117">The identifier of any policy that was created by applying the workload action.</span></span> <span data-ttu-id="11846-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="11846-118">Optional.</span></span> <span data-ttu-id="11846-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11846-119">Read-only.</span></span>|
|<span data-ttu-id="11846-120">error</span><span class="sxs-lookup"><span data-stu-id="11846-120">error</span></span>|[<span data-ttu-id="11846-121">microsoft.graph.genericError</span><span class="sxs-lookup"><span data-stu-id="11846-121">microsoft.graph.genericError</span></span>](../resources/genericerror.md)|<span data-ttu-id="11846-122">Подробные сведения об исключениях, которые возникают при развертывании действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="11846-122">The detailed information for exceptions that occur when deploying the workload action.</span></span> <span data-ttu-id="11846-123">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="11846-123">Optional.</span></span> <span data-ttu-id="11846-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11846-124">Required.</span></span>|
|<span data-ttu-id="11846-125">lastDeploymentDateTime</span><span class="sxs-lookup"><span data-stu-id="11846-125">lastDeploymentDateTime</span></span>|<span data-ttu-id="11846-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11846-126">DateTimeOffset</span></span>|<span data-ttu-id="11846-127">Дата и время последнего развертывания действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="11846-127">The date and time the workload action was last deployed.</span></span> <span data-ttu-id="11846-128">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="11846-128">Optional.</span></span>|
|<span data-ttu-id="11846-129">status</span><span class="sxs-lookup"><span data-stu-id="11846-129">status</span></span>|<span data-ttu-id="11846-130">workloadActionStatus</span><span class="sxs-lookup"><span data-stu-id="11846-130">workloadActionStatus</span></span>|<span data-ttu-id="11846-131">Состояние развертывания действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="11846-131">The status of the workload action deployment.</span></span> <span data-ttu-id="11846-132">Возможные значения: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="11846-132">Possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `unknownFutureValue`.</span></span> <span data-ttu-id="11846-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11846-133">Required.</span></span> <span data-ttu-id="11846-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11846-134">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11846-135">Связи</span><span class="sxs-lookup"><span data-stu-id="11846-135">Relationships</span></span>
<span data-ttu-id="11846-136">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="11846-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11846-137">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="11846-137">JSON representation</span></span>
<span data-ttu-id="11846-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11846-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadActionDeploymentStatus",
  "actionId": "String",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.genericError"
  },
  "deployedPolicyId": "String",
  "lastDeploymentDateTime": "String (timestamp)"
}
```
