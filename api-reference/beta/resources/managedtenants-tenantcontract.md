---
title: тип ресурса tenantContract
description: Представляет сведения о связи между клиентом и управляющей организацией.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 104b475428efe82a2e56f823845b933149aeab18
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402699"
---
# <a name="tenantcontract-resource-type"></a><span data-ttu-id="e90dd-103">тип ресурса tenantContract</span><span class="sxs-lookup"><span data-stu-id="e90dd-103">tenantContract resource type</span></span>

<span data-ttu-id="e90dd-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e90dd-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e90dd-105">Представляет сведения о связи между клиентом и управляющей организацией.</span><span class="sxs-lookup"><span data-stu-id="e90dd-105">Represents relationship information between a tenant and the managing entity.</span></span>

## <a name="properties"></a><span data-ttu-id="e90dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e90dd-106">Properties</span></span>
|<span data-ttu-id="e90dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e90dd-107">Property</span></span>|<span data-ttu-id="e90dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e90dd-108">Type</span></span>|<span data-ttu-id="e90dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e90dd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e90dd-110">contractType</span><span class="sxs-lookup"><span data-stu-id="e90dd-110">contractType</span></span>|<span data-ttu-id="e90dd-111">Int32</span><span class="sxs-lookup"><span data-stu-id="e90dd-111">Int32</span></span>|<span data-ttu-id="e90dd-112">Тип отношений, которые существуют между управляющей сущностью и клиентом.</span><span class="sxs-lookup"><span data-stu-id="e90dd-112">The type of relationship that exists between the managing entity and tenant.</span></span> <span data-ttu-id="e90dd-113">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e90dd-113">Optional.</span></span> <span data-ttu-id="e90dd-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e90dd-114">Read-only.</span></span>|
|<span data-ttu-id="e90dd-115">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="e90dd-115">defaultDomainName</span></span>|<span data-ttu-id="e90dd-116">String</span><span class="sxs-lookup"><span data-stu-id="e90dd-116">String</span></span>|<span data-ttu-id="e90dd-117">Доменное имя по умолчанию для клиента.</span><span class="sxs-lookup"><span data-stu-id="e90dd-117">The default domain name for the tenant.</span></span> <span data-ttu-id="e90dd-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e90dd-118">Required.</span></span> <span data-ttu-id="e90dd-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e90dd-119">Read-only.</span></span>|
|<span data-ttu-id="e90dd-120">displayName</span><span class="sxs-lookup"><span data-stu-id="e90dd-120">displayName</span></span>|<span data-ttu-id="e90dd-121">String</span><span class="sxs-lookup"><span data-stu-id="e90dd-121">String</span></span>|<span data-ttu-id="e90dd-122">Отображаемое имя для клиента.</span><span class="sxs-lookup"><span data-stu-id="e90dd-122">The display name for the tenant.</span></span> <span data-ttu-id="e90dd-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e90dd-123">Optional.</span></span> <span data-ttu-id="e90dd-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e90dd-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e90dd-125">Связи</span><span class="sxs-lookup"><span data-stu-id="e90dd-125">Relationships</span></span>
<span data-ttu-id="e90dd-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e90dd-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e90dd-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e90dd-127">JSON representation</span></span>
<span data-ttu-id="e90dd-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e90dd-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContract"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContract",
  "contractType": "Integer",
  "displayName": "String",
  "defaultDomainName": "String"
}
```
