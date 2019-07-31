---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 091bb8e6c1a14f6c173d18acf68679feb6c88eaf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964231"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="03e91-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="03e91-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03e91-105">Задает домен клиента.</span><span class="sxs-lookup"><span data-stu-id="03e91-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="03e91-106">Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="03e91-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="03e91-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="03e91-107">Properties</span></span>
| <span data-ttu-id="03e91-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="03e91-108">Property</span></span>     | <span data-ttu-id="03e91-109">Тип</span><span class="sxs-lookup"><span data-stu-id="03e91-109">Type</span></span>   |<span data-ttu-id="03e91-110">Описание</span><span class="sxs-lookup"><span data-stu-id="03e91-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03e91-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="03e91-111">capabilities</span></span>|<span data-ttu-id="03e91-112">String</span><span class="sxs-lookup"><span data-stu-id="03e91-112">String</span></span>|<span data-ttu-id="03e91-113">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="03e91-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="03e91-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="03e91-114">isDefault</span></span>|<span data-ttu-id="03e91-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e91-115">Boolean</span></span>|                <span data-ttu-id="03e91-116">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="03e91-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="03e91-117">при инициализации</span><span class="sxs-lookup"><span data-stu-id="03e91-117">isInitial</span></span>|<span data-ttu-id="03e91-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e91-118">Boolean</span></span>|<span data-ttu-id="03e91-119">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="03e91-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="03e91-120">name</span><span class="sxs-lookup"><span data-stu-id="03e91-120">name</span></span>|<span data-ttu-id="03e91-121">String</span><span class="sxs-lookup"><span data-stu-id="03e91-121">String</span></span>|<span data-ttu-id="03e91-122">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="03e91-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="03e91-123">type</span><span class="sxs-lookup"><span data-stu-id="03e91-123">type</span></span>|<span data-ttu-id="03e91-124">String</span><span class="sxs-lookup"><span data-stu-id="03e91-124">String</span></span>|<span data-ttu-id="03e91-125">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="03e91-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03e91-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03e91-126">JSON representation</span></span>

<span data-ttu-id="03e91-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03e91-127">Here is a JSON representation of the resource</span></span>

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
