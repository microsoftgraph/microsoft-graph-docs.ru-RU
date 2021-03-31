---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: b4a3a5bed105fe0e0849ddf7c21d7a1b087942ca
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468686"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="1a2eb-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="1a2eb-104">verifiedDomain resource type</span></span>

<span data-ttu-id="1a2eb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a2eb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a2eb-106">Задает домен клиента.</span><span class="sxs-lookup"><span data-stu-id="1a2eb-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="1a2eb-107">Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="1a2eb-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="1a2eb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a2eb-108">Properties</span></span>
| <span data-ttu-id="1a2eb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a2eb-109">Property</span></span>     | <span data-ttu-id="1a2eb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1a2eb-110">Type</span></span>   |<span data-ttu-id="1a2eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a2eb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a2eb-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="1a2eb-112">capabilities</span></span>|<span data-ttu-id="1a2eb-113">String</span><span class="sxs-lookup"><span data-stu-id="1a2eb-113">String</span></span>|<span data-ttu-id="1a2eb-114">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="1a2eb-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="1a2eb-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="1a2eb-115">isDefault</span></span>|<span data-ttu-id="1a2eb-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a2eb-116">Boolean</span></span>|                <span data-ttu-id="1a2eb-117">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="1a2eb-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="1a2eb-118">isInitial</span><span class="sxs-lookup"><span data-stu-id="1a2eb-118">isInitial</span></span>|<span data-ttu-id="1a2eb-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a2eb-119">Boolean</span></span>|<span data-ttu-id="1a2eb-120">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="1a2eb-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="1a2eb-121">name</span><span class="sxs-lookup"><span data-stu-id="1a2eb-121">name</span></span>|<span data-ttu-id="1a2eb-122">String</span><span class="sxs-lookup"><span data-stu-id="1a2eb-122">String</span></span>|<span data-ttu-id="1a2eb-123">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="1a2eb-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="1a2eb-124">type</span><span class="sxs-lookup"><span data-stu-id="1a2eb-124">type</span></span>|<span data-ttu-id="1a2eb-125">String</span><span class="sxs-lookup"><span data-stu-id="1a2eb-125">String</span></span>|<span data-ttu-id="1a2eb-126">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="1a2eb-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a2eb-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a2eb-127">JSON representation</span></span>

<span data-ttu-id="1a2eb-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a2eb-128">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


