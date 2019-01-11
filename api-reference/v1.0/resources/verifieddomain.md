---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
ms.openlocfilehash: 6eb6490ce8dac29f2617b7873230fad7c7b5c536
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876498"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="685e4-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="685e4-104">verifiedDomain resource type</span></span>

<span data-ttu-id="685e4-p102">Задает домен клиента. Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="685e4-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="685e4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="685e4-107">Properties</span></span>
| <span data-ttu-id="685e4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="685e4-108">Property</span></span>     | <span data-ttu-id="685e4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="685e4-109">Type</span></span>   |<span data-ttu-id="685e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="685e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="685e4-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="685e4-111">capabilities</span></span>|<span data-ttu-id="685e4-112">String</span><span class="sxs-lookup"><span data-stu-id="685e4-112">String</span></span>|<span data-ttu-id="685e4-113">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="685e4-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="685e4-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="685e4-114">isDefault</span></span>|<span data-ttu-id="685e4-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="685e4-115">Boolean</span></span>|                <span data-ttu-id="685e4-116">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="685e4-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="685e4-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="685e4-117">isInitial</span></span>|<span data-ttu-id="685e4-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="685e4-118">Boolean</span></span>|<span data-ttu-id="685e4-119">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="685e4-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="685e4-120">name</span><span class="sxs-lookup"><span data-stu-id="685e4-120">name</span></span>|<span data-ttu-id="685e4-121">String</span><span class="sxs-lookup"><span data-stu-id="685e4-121">String</span></span>|<span data-ttu-id="685e4-122">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="685e4-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="685e4-123">type</span><span class="sxs-lookup"><span data-stu-id="685e4-123">type</span></span>|<span data-ttu-id="685e4-124">String</span><span class="sxs-lookup"><span data-stu-id="685e4-124">String</span></span>|<span data-ttu-id="685e4-125">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="685e4-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="685e4-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="685e4-126">JSON representation</span></span>

<span data-ttu-id="685e4-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="685e4-127">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
