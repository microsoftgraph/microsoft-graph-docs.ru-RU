---
title: тип ресурса workloadAction
description: Представляет действие, которое будет выполняться для определенной рабочей нагрузки.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e6dbbe1458aa6dba37a26af70ee0e64b92a52cf4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402598"
---
# <a name="workloadaction-resource-type"></a><span data-ttu-id="c96aa-103">тип ресурса workloadAction</span><span class="sxs-lookup"><span data-stu-id="c96aa-103">workloadAction resource type</span></span>

<span data-ttu-id="c96aa-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c96aa-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c96aa-105">Представляет действие, которое будет выполняться для определенной рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c96aa-105">Represents an action that will be performed for a specific workload.</span></span>

## <a name="properties"></a><span data-ttu-id="c96aa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c96aa-106">Properties</span></span>
|<span data-ttu-id="c96aa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c96aa-107">Property</span></span>|<span data-ttu-id="c96aa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c96aa-108">Type</span></span>|<span data-ttu-id="c96aa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c96aa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c96aa-110">actionId</span><span class="sxs-lookup"><span data-stu-id="c96aa-110">actionId</span></span>|<span data-ttu-id="c96aa-111">String</span><span class="sxs-lookup"><span data-stu-id="c96aa-111">String</span></span>|<span data-ttu-id="c96aa-112">Уникальный идентификатор для действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c96aa-112">The unique identifier for the workload action.</span></span> <span data-ttu-id="c96aa-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c96aa-113">Required.</span></span> <span data-ttu-id="c96aa-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c96aa-114">Read-only.</span></span>|
|<span data-ttu-id="c96aa-115">category</span><span class="sxs-lookup"><span data-stu-id="c96aa-115">category</span></span>|<span data-ttu-id="c96aa-116">workloadActionCategory</span><span class="sxs-lookup"><span data-stu-id="c96aa-116">workloadActionCategory</span></span>|<span data-ttu-id="c96aa-117">Категория действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c96aa-117">The category for the workload action.</span></span> <span data-ttu-id="c96aa-118">Возможные значения: `automated`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c96aa-118">Possible values are: `automated`, `manual`, `unknownFutureValue`.</span></span> <span data-ttu-id="c96aa-119">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c96aa-119">Optional.</span></span> <span data-ttu-id="c96aa-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c96aa-120">Read-only.</span></span>|
|<span data-ttu-id="c96aa-121">description</span><span class="sxs-lookup"><span data-stu-id="c96aa-121">description</span></span>|<span data-ttu-id="c96aa-122">String</span><span class="sxs-lookup"><span data-stu-id="c96aa-122">String</span></span>|<span data-ttu-id="c96aa-123">Описание действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c96aa-123">The description for the workload action.</span></span> <span data-ttu-id="c96aa-124">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c96aa-124">Optional.</span></span> <span data-ttu-id="c96aa-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c96aa-125">Read-only.</span></span>|
|<span data-ttu-id="c96aa-126">displayName</span><span class="sxs-lookup"><span data-stu-id="c96aa-126">displayName</span></span>|<span data-ttu-id="c96aa-127">String</span><span class="sxs-lookup"><span data-stu-id="c96aa-127">String</span></span>|<span data-ttu-id="c96aa-128">Отображает имя для действия рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c96aa-128">The display name for the workload action.</span></span> <span data-ttu-id="c96aa-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c96aa-129">Optional.</span></span> <span data-ttu-id="c96aa-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c96aa-130">Read-only.</span></span>|
|<span data-ttu-id="c96aa-131">service</span><span class="sxs-lookup"><span data-stu-id="c96aa-131">service</span></span>|<span data-ttu-id="c96aa-132">String</span><span class="sxs-lookup"><span data-stu-id="c96aa-132">String</span></span>|<span data-ttu-id="c96aa-133">Служба, связанная с действием рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c96aa-133">The service associated with workload action.</span></span> <span data-ttu-id="c96aa-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c96aa-134">Optional.</span></span> <span data-ttu-id="c96aa-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c96aa-135">Read-only.</span></span>|
|<span data-ttu-id="c96aa-136">settings</span><span class="sxs-lookup"><span data-stu-id="c96aa-136">settings</span></span>|<span data-ttu-id="c96aa-137">[коллекция microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md)</span><span class="sxs-lookup"><span data-stu-id="c96aa-137">[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection</span></span>|<span data-ttu-id="c96aa-138">Коллекция параметров, связанных с действием рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="c96aa-138">The collection of settings associated with the workload action.</span></span> <span data-ttu-id="c96aa-139">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c96aa-139">Optional.</span></span> <span data-ttu-id="c96aa-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c96aa-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c96aa-141">Связи</span><span class="sxs-lookup"><span data-stu-id="c96aa-141">Relationships</span></span>
<span data-ttu-id="c96aa-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c96aa-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c96aa-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c96aa-143">JSON representation</span></span>
<span data-ttu-id="c96aa-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c96aa-144">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadAction",
  "actionId": "String",
  "category": "String",
  "displayName": "String",
  "description": "String",
  "service": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ]
}
```
