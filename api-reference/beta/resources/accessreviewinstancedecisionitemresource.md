---
title: accessReviewInstanceDecisionItemResource type
description: Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу. accessReviewInstanceDecisionItemResource представляет ресурс, связанный с элементом решения.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 879a0b1f74fa08e0ae66e5aaf5ab45b9d96de397
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469791"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a><span data-ttu-id="05238-104">accessReviewInstanceDecisionItemResource type</span><span class="sxs-lookup"><span data-stu-id="05238-104">accessReviewInstanceDecisionItemResource resource type</span></span>

<span data-ttu-id="05238-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05238-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="05238-106">Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="05238-106">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="05238-107">accessReviewInstanceDecisionItemResource представляет ресурс, связанный с элементом решения.</span><span class="sxs-lookup"><span data-stu-id="05238-107">accessReviewInstanceDecisionItemResource represents the resource associated with the decision item.</span></span>

## <a name="properties"></a><span data-ttu-id="05238-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="05238-108">Properties</span></span>
|<span data-ttu-id="05238-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="05238-109">Property</span></span>|<span data-ttu-id="05238-110">Тип</span><span class="sxs-lookup"><span data-stu-id="05238-110">Type</span></span>|<span data-ttu-id="05238-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05238-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05238-112">displayName</span><span class="sxs-lookup"><span data-stu-id="05238-112">displayName</span></span>|<span data-ttu-id="05238-113">String</span><span class="sxs-lookup"><span data-stu-id="05238-113">String</span></span>|<span data-ttu-id="05238-114">Отображение имени ресурса</span><span class="sxs-lookup"><span data-stu-id="05238-114">Display name of the resource</span></span>|
|<span data-ttu-id="05238-115">id</span><span class="sxs-lookup"><span data-stu-id="05238-115">id</span></span>|<span data-ttu-id="05238-116">String</span><span class="sxs-lookup"><span data-stu-id="05238-116">String</span></span>|<span data-ttu-id="05238-117">ИД ресурса</span><span class="sxs-lookup"><span data-stu-id="05238-117">Resource ID</span></span>|
|<span data-ttu-id="05238-118">type</span><span class="sxs-lookup"><span data-stu-id="05238-118">type</span></span>|<span data-ttu-id="05238-119">String</span><span class="sxs-lookup"><span data-stu-id="05238-119">String</span></span>|<span data-ttu-id="05238-120">Тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="05238-120">Type of resource.</span></span> <span data-ttu-id="05238-121">Типы включают: Group, ServicePrincipal, DirectoryRole, AzureRole, AccessPackageAssignmentPolicy.</span><span class="sxs-lookup"><span data-stu-id="05238-121">Types include: Group, ServicePrincipal, DirectoryRole, AzureRole, AccessPackageAssignmentPolicy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05238-122">Связи</span><span class="sxs-lookup"><span data-stu-id="05238-122">Relationships</span></span>
<span data-ttu-id="05238-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="05238-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05238-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="05238-124">JSON representation</span></span>
<span data-ttu-id="05238-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05238-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String"
}
```
