---
title: тип ресурса conditionalAccessPolicyCoverage
description: Представляет сведения о любой политике Azure Active Directory, определяемой правилами доступа к ресурсу для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a4bc4f336692166ff032727a6fb13222edd9d7d9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402543"
---
# <a name="conditionalaccesspolicycoverage-resource-type"></a><span data-ttu-id="e7500-103">тип ресурса conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="e7500-103">conditionalAccessPolicyCoverage resource type</span></span>

<span data-ttu-id="e7500-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e7500-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7500-105">Представляет сведения о любой политике Azure Active Directory, определяемой правилами доступа к ресурсу для данного управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="e7500-105">Represents information about any Azure Active Directory policy that defines access rules of a resource for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="e7500-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e7500-106">Methods</span></span>
|<span data-ttu-id="e7500-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e7500-107">Method</span></span>|<span data-ttu-id="e7500-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e7500-108">Return type</span></span>|<span data-ttu-id="e7500-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e7500-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e7500-110">Список conditionalAccessPolicyCoverages</span><span class="sxs-lookup"><span data-stu-id="e7500-110">List conditionalAccessPolicyCoverages</span></span>](../api/managedtenants-managedtenant-list-conditionalaccesspolicycoverages.md)|<span data-ttu-id="e7500-111">[коллекция microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)</span><span class="sxs-lookup"><span data-stu-id="e7500-111">[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) collection</span></span>|<span data-ttu-id="e7500-112">Получите список объектов [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="e7500-112">Get a list of the [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) objects and their properties.</span></span>|
|[<span data-ttu-id="e7500-113">Get conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="e7500-113">Get conditionalAccessPolicyCoverage</span></span>](../api/managedtenants-conditionalaccesspolicycoverage-get.md)|[<span data-ttu-id="e7500-114">microsoft.graph.managedTenants.conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="e7500-114">microsoft.graph.managedTenants.conditionalAccessPolicyCoverage</span></span>](../resources/managedtenants-conditionalaccesspolicycoverage.md)|<span data-ttu-id="e7500-115">Ознакомьтесь с свойствами и отношениями объекта [conditionalAccessPolicyCoverage.](../resources/managedtenants-conditionalaccesspolicycoverage.md)</span><span class="sxs-lookup"><span data-stu-id="e7500-115">Read the properties and relationships of a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e7500-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7500-116">Properties</span></span>
|<span data-ttu-id="e7500-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7500-117">Property</span></span>|<span data-ttu-id="e7500-118">Тип</span><span class="sxs-lookup"><span data-stu-id="e7500-118">Type</span></span>|<span data-ttu-id="e7500-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e7500-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7500-120">conditionalAccessPolicyState</span><span class="sxs-lookup"><span data-stu-id="e7500-120">conditionalAccessPolicyState</span></span>|<span data-ttu-id="e7500-121">String</span><span class="sxs-lookup"><span data-stu-id="e7500-121">String</span></span>|<span data-ttu-id="e7500-122">Состояние политики условного доступа.</span><span class="sxs-lookup"><span data-stu-id="e7500-122">The state for the conditional access policy.</span></span> <span data-ttu-id="e7500-123">Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span><span class="sxs-lookup"><span data-stu-id="e7500-123">Possible values are: `enabled`, `disabled`, `enabledForReportingButNotEnforced`.</span></span> <span data-ttu-id="e7500-124">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="e7500-124">Required.</span></span> <span data-ttu-id="e7500-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7500-125">Read-only.</span></span>|
|<span data-ttu-id="e7500-126">id</span><span class="sxs-lookup"><span data-stu-id="e7500-126">id</span></span>|<span data-ttu-id="e7500-127">String</span><span class="sxs-lookup"><span data-stu-id="e7500-127">String</span></span>|<span data-ttu-id="e7500-128">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="e7500-128">The unique identifier for this entity.</span></span> <span data-ttu-id="e7500-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7500-129">Required.</span></span> <span data-ttu-id="e7500-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7500-130">Read-only.</span></span>|
|<span data-ttu-id="e7500-131">latestPolicyModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7500-131">latestPolicyModifiedDateTime</span></span>|<span data-ttu-id="e7500-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7500-132">DateTimeOffset</span></span>|<span data-ttu-id="e7500-133">Дата и время последнего изменения политики условного доступа.</span><span class="sxs-lookup"><span data-stu-id="e7500-133">The date and time the conditional access policy was last modified.</span></span> <span data-ttu-id="e7500-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7500-134">Required.</span></span> <span data-ttu-id="e7500-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7500-135">Read-only.</span></span>|
|<span data-ttu-id="e7500-136">requiresDeviceCompliance</span><span class="sxs-lookup"><span data-stu-id="e7500-136">requiresDeviceCompliance</span></span>|<span data-ttu-id="e7500-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7500-137">Boolean</span></span>|<span data-ttu-id="e7500-138">Флаг, указывающий, требуется ли политике условного доступа соответствие требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="e7500-138">A flag indicating whether the conditional access policy requires device compliance.</span></span> <span data-ttu-id="e7500-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7500-139">Required.</span></span> <span data-ttu-id="e7500-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7500-140">Read-only.</span></span>|
|<span data-ttu-id="e7500-141">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="e7500-141">tenantDisplayName</span></span>|<span data-ttu-id="e7500-142">String</span><span class="sxs-lookup"><span data-stu-id="e7500-142">String</span></span>|<span data-ttu-id="e7500-143">Имя отображения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="e7500-143">The display name for the managed tenant.</span></span> <span data-ttu-id="e7500-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7500-144">Required.</span></span> <span data-ttu-id="e7500-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7500-145">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7500-146">Связи</span><span class="sxs-lookup"><span data-stu-id="e7500-146">Relationships</span></span>
<span data-ttu-id="e7500-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e7500-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7500-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e7500-148">JSON representation</span></span>
<span data-ttu-id="e7500-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7500-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```
