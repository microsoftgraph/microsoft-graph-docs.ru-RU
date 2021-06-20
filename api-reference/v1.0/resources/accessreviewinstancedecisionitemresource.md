---
title: accessReviewInstanceDecisionItemResource type
description: Представляет ресурс, связанный с элементом решения.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d75fb2f2b2fd4338f63d2c71893f2dab17524bc8
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031242"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a><span data-ttu-id="8e3dd-103">accessReviewInstanceDecisionItemResource type</span><span class="sxs-lookup"><span data-stu-id="8e3dd-103">accessReviewInstanceDecisionItemResource resource type</span></span>

<span data-ttu-id="8e3dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e3dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e3dd-105">Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="8e3dd-105">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="8e3dd-106">Объект accessReviewInstanceDecisionItemResource представляет ресурс, связанный с элементом решения.</span><span class="sxs-lookup"><span data-stu-id="8e3dd-106">The accessReviewInstanceDecisionItemResource object represents the resource associated with the decision item.</span></span>

## <a name="properties"></a><span data-ttu-id="8e3dd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e3dd-107">Properties</span></span>
|<span data-ttu-id="8e3dd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e3dd-108">Property</span></span>|<span data-ttu-id="8e3dd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8e3dd-109">Type</span></span>|<span data-ttu-id="8e3dd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8e3dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e3dd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8e3dd-111">displayName</span></span>|<span data-ttu-id="8e3dd-112">String</span><span class="sxs-lookup"><span data-stu-id="8e3dd-112">String</span></span>|<span data-ttu-id="8e3dd-113">Отображение имени ресурса</span><span class="sxs-lookup"><span data-stu-id="8e3dd-113">Display name of the resource</span></span>|
|<span data-ttu-id="8e3dd-114">id</span><span class="sxs-lookup"><span data-stu-id="8e3dd-114">id</span></span>|<span data-ttu-id="8e3dd-115">String</span><span class="sxs-lookup"><span data-stu-id="8e3dd-115">String</span></span>|<span data-ttu-id="8e3dd-116">Идентификатор ресурса</span><span class="sxs-lookup"><span data-stu-id="8e3dd-116">Identifier of the resource</span></span>|
|<span data-ttu-id="8e3dd-117">type</span><span class="sxs-lookup"><span data-stu-id="8e3dd-117">type</span></span>|<span data-ttu-id="8e3dd-118">String</span><span class="sxs-lookup"><span data-stu-id="8e3dd-118">String</span></span>|<span data-ttu-id="8e3dd-119">Тип ресурса.</span><span class="sxs-lookup"><span data-stu-id="8e3dd-119">Type of resource.</span></span> <span data-ttu-id="8e3dd-120">Типы включают: `Group` , , , , `ServicePrincipal` `DirectoryRole` `AzureRole` `AccessPackageAssignmentPolicy` .</span><span class="sxs-lookup"><span data-stu-id="8e3dd-120">Types include: `Group`, `ServicePrincipal`, `DirectoryRole`, `AzureRole`, `AccessPackageAssignmentPolicy`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e3dd-121">Связи</span><span class="sxs-lookup"><span data-stu-id="8e3dd-121">Relationships</span></span>
<span data-ttu-id="8e3dd-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8e3dd-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e3dd-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8e3dd-123">JSON representation</span></span>
<span data-ttu-id="8e3dd-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e3dd-124">The following is a JSON representation of the resource.</span></span>
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
