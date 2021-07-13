---
title: тип ресурсов managementTemplate
description: Представляет группу действий и параметр, которые можно выполнить в отношении управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2055db2d291dce3da0b4ad144c07b09bbb2fea6f
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402700"
---
# <a name="managementtemplate-resource-type"></a><span data-ttu-id="76d70-103">тип ресурсов managementTemplate</span><span class="sxs-lookup"><span data-stu-id="76d70-103">managementTemplate resource type</span></span>

<span data-ttu-id="76d70-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="76d70-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76d70-105">Представляет группу действий и параметр, которые можно выполнить в отношении управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="76d70-105">Represents a group of actions and setting that can be performed against a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="76d70-106">Методы</span><span class="sxs-lookup"><span data-stu-id="76d70-106">Methods</span></span>
|<span data-ttu-id="76d70-107">Метод</span><span class="sxs-lookup"><span data-stu-id="76d70-107">Method</span></span>|<span data-ttu-id="76d70-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="76d70-108">Return type</span></span>|<span data-ttu-id="76d70-109">Описание</span><span class="sxs-lookup"><span data-stu-id="76d70-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76d70-110">Управление спискамиTemplates</span><span class="sxs-lookup"><span data-stu-id="76d70-110">List managementTemplates</span></span>](../api/managedtenants-managedtenant-list-managementtemplates.md)|<span data-ttu-id="76d70-111">[коллекция microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="76d70-111">[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) collection</span></span>|<span data-ttu-id="76d70-112">Получите список объектов [managementTemplate](../resources/managedtenants-managementtemplate.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="76d70-112">Get a list of the [managementTemplate](../resources/managedtenants-managementtemplate.md) objects and their properties.</span></span>|
|[<span data-ttu-id="76d70-113">Get managementTemplate</span><span class="sxs-lookup"><span data-stu-id="76d70-113">Get managementTemplate</span></span>](../api/managedtenants-managementtemplate-get.md)|[<span data-ttu-id="76d70-114">microsoft.graph.managedTenants.managementTemplate</span><span class="sxs-lookup"><span data-stu-id="76d70-114">microsoft.graph.managedTenants.managementTemplate</span></span>](../resources/managedtenants-managementtemplate.md)|<span data-ttu-id="76d70-115">Ознакомьтесь с свойствами и отношениями [объекта managementTemplate.](../resources/managedtenants-managementtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="76d70-115">Read the properties and relationships of a [managementTemplate](../resources/managedtenants-managementtemplate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="76d70-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="76d70-116">Properties</span></span>
|<span data-ttu-id="76d70-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="76d70-117">Property</span></span>|<span data-ttu-id="76d70-118">Тип</span><span class="sxs-lookup"><span data-stu-id="76d70-118">Type</span></span>|<span data-ttu-id="76d70-119">Описание</span><span class="sxs-lookup"><span data-stu-id="76d70-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76d70-120">category</span><span class="sxs-lookup"><span data-stu-id="76d70-120">category</span></span>|<span data-ttu-id="76d70-121">managementCategory</span><span class="sxs-lookup"><span data-stu-id="76d70-121">managementCategory</span></span>|<span data-ttu-id="76d70-122">Категория управления для шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="76d70-122">The management category for the management template.</span></span> <span data-ttu-id="76d70-123">Возможные значения: `custom`, `devices`, `identity`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="76d70-123">Possible values are: `custom`, `devices`, `identity`, `unknownFutureValue`.</span></span> <span data-ttu-id="76d70-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76d70-124">Required.</span></span> <span data-ttu-id="76d70-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d70-125">Read-only.</span></span>|
|<span data-ttu-id="76d70-126">description</span><span class="sxs-lookup"><span data-stu-id="76d70-126">description</span></span>|<span data-ttu-id="76d70-127">String</span><span class="sxs-lookup"><span data-stu-id="76d70-127">String</span></span>|<span data-ttu-id="76d70-128">Описание шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="76d70-128">The description for the management template.</span></span> <span data-ttu-id="76d70-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="76d70-129">Optional.</span></span> <span data-ttu-id="76d70-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d70-130">Read-only.</span></span>|
|<span data-ttu-id="76d70-131">displayName</span><span class="sxs-lookup"><span data-stu-id="76d70-131">displayName</span></span>|<span data-ttu-id="76d70-132">String</span><span class="sxs-lookup"><span data-stu-id="76d70-132">String</span></span>|<span data-ttu-id="76d70-133">Имя отображения шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="76d70-133">The display name for the management template.</span></span> <span data-ttu-id="76d70-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76d70-134">Required.</span></span> <span data-ttu-id="76d70-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d70-135">Read-only.</span></span>|
|<span data-ttu-id="76d70-136">id</span><span class="sxs-lookup"><span data-stu-id="76d70-136">id</span></span>|<span data-ttu-id="76d70-137">String</span><span class="sxs-lookup"><span data-stu-id="76d70-137">String</span></span>|<span data-ttu-id="76d70-138">Уникальный идентификатор шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="76d70-138">The unique identifier for the management template.</span></span> <span data-ttu-id="76d70-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76d70-139">Required.</span></span> <span data-ttu-id="76d70-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d70-140">Read-only.</span></span>|
|<span data-ttu-id="76d70-141">parameters</span><span class="sxs-lookup"><span data-stu-id="76d70-141">parameters</span></span>|<span data-ttu-id="76d70-142">[коллекция microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md)</span><span class="sxs-lookup"><span data-stu-id="76d70-142">[microsoft.graph.managedTenants.templateParameter](../resources/managedtenants-templateparameter.md) collection</span></span>|<span data-ttu-id="76d70-143">Коллекция параметров, используемых шаблоном управления.</span><span class="sxs-lookup"><span data-stu-id="76d70-143">The collection of parameters used by the management template.</span></span> <span data-ttu-id="76d70-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="76d70-144">Optional.</span></span> <span data-ttu-id="76d70-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d70-145">Read-only.</span></span>|
|<span data-ttu-id="76d70-146">workloadActions</span><span class="sxs-lookup"><span data-stu-id="76d70-146">workloadActions</span></span>|<span data-ttu-id="76d70-147">[коллекция microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md)</span><span class="sxs-lookup"><span data-stu-id="76d70-147">[microsoft.graph.managedTenants.workloadAction](../resources/managedtenants-workloadaction.md) collection</span></span>|<span data-ttu-id="76d70-148">Набор действий рабочей нагрузки, связанных с шаблоном управления.</span><span class="sxs-lookup"><span data-stu-id="76d70-148">The collection of workload actions associated with the management template.</span></span> <span data-ttu-id="76d70-149">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="76d70-149">Optional.</span></span> <span data-ttu-id="76d70-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d70-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76d70-151">Связи</span><span class="sxs-lookup"><span data-stu-id="76d70-151">Relationships</span></span>
<span data-ttu-id="76d70-152">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="76d70-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76d70-153">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="76d70-153">JSON representation</span></span>
<span data-ttu-id="76d70-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76d70-154">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managementTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "category": "String",
  "parameters": [
    {
      "@odata.type": "microsoft.graph.managedTenants.templateParameter"
    }
  ],
  "workloadActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadAction"
    }
  ]
}
```
