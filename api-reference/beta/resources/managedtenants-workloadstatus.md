---
title: тип ресурса workloadStatus
description: Представляет состояние рабочей нагрузки.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 50cbd9cdc59426f413333835c4418112401d8038
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403132"
---
# <a name="workloadstatus-resource-type"></a><span data-ttu-id="209a3-103">тип ресурса workloadStatus</span><span class="sxs-lookup"><span data-stu-id="209a3-103">workloadStatus resource type</span></span>

<span data-ttu-id="209a3-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="209a3-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="209a3-105">Представляет состояние рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="209a3-105">Represent the status for a workload.</span></span>

## <a name="properties"></a><span data-ttu-id="209a3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="209a3-106">Properties</span></span>
|<span data-ttu-id="209a3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="209a3-107">Property</span></span>|<span data-ttu-id="209a3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="209a3-108">Type</span></span>|<span data-ttu-id="209a3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="209a3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="209a3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="209a3-110">displayName</span></span>|<span data-ttu-id="209a3-111">String</span><span class="sxs-lookup"><span data-stu-id="209a3-111">String</span></span>|<span data-ttu-id="209a3-112">Имя отображения рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="209a3-112">The display name for the workload.</span></span> <span data-ttu-id="209a3-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="209a3-113">Required.</span></span> <span data-ttu-id="209a3-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="209a3-114">Read-only.</span></span>|
|<span data-ttu-id="209a3-115">offboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="209a3-115">offboardedDateTime</span></span>|<span data-ttu-id="209a3-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="209a3-116">DateTimeOffset</span></span>|<span data-ttu-id="209a3-117">Дата и время отключения рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="209a3-117">The date and time the workload was offboarded.</span></span> <span data-ttu-id="209a3-118">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="209a3-118">Optional.</span></span> <span data-ttu-id="209a3-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="209a3-119">Read-only.</span></span>|
|<span data-ttu-id="209a3-120">onboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="209a3-120">onboardedDateTime</span></span>|<span data-ttu-id="209a3-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="209a3-121">DateTimeOffset</span></span>|<span data-ttu-id="209a3-122">Дата и время загрузки.</span><span class="sxs-lookup"><span data-stu-id="209a3-122">The date and time the workload was onboarded.</span></span> <span data-ttu-id="209a3-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="209a3-123">Optional.</span></span> <span data-ttu-id="209a3-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="209a3-124">Read-only.</span></span>|
|<span data-ttu-id="209a3-125">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="209a3-125">onboardingStatus</span></span>|<span data-ttu-id="209a3-126">workloadOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="209a3-126">workloadOnboardingStatus</span></span>|<span data-ttu-id="209a3-127">Состояние onboarding для рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="209a3-127">The onboarding status for the workload.</span></span> <span data-ttu-id="209a3-128">Возможные значения: `notOnboarded`, `onboarded`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="209a3-128">Possible values are: `notOnboarded`, `onboarded`, `unknownFutureValue`.</span></span> <span data-ttu-id="209a3-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="209a3-129">Optional.</span></span> <span data-ttu-id="209a3-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="209a3-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="209a3-131">Связи</span><span class="sxs-lookup"><span data-stu-id="209a3-131">Relationships</span></span>
<span data-ttu-id="209a3-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="209a3-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="209a3-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="209a3-133">JSON representation</span></span>
<span data-ttu-id="209a3-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="209a3-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadStatus",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "displayName": "String",
  "offboardedDateTime": "String (timestamp)"
}
```
