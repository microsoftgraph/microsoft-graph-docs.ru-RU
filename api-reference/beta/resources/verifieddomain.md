---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
ms.openlocfilehash: 810b5fea0fbaf82eeb452c0f5c6032679590ff49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080099"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="87cdf-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="87cdf-104">verifiedDomain resource type</span></span>

> <span data-ttu-id="87cdf-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="87cdf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87cdf-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87cdf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87cdf-p103">Задает домен клиента. Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="87cdf-p103">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="87cdf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="87cdf-109">Properties</span></span>
| <span data-ttu-id="87cdf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="87cdf-110">Property</span></span>     | <span data-ttu-id="87cdf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="87cdf-111">Type</span></span>   |<span data-ttu-id="87cdf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="87cdf-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87cdf-113">capabilities</span><span class="sxs-lookup"><span data-stu-id="87cdf-113">capabilities</span></span>|<span data-ttu-id="87cdf-114">String</span><span class="sxs-lookup"><span data-stu-id="87cdf-114">String</span></span>|<span data-ttu-id="87cdf-115">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="87cdf-115">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="87cdf-116">isDefault</span><span class="sxs-lookup"><span data-stu-id="87cdf-116">isDefault</span></span>|<span data-ttu-id="87cdf-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="87cdf-117">Boolean</span></span>|                <span data-ttu-id="87cdf-118">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="87cdf-118">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="87cdf-119">isInitial</span><span class="sxs-lookup"><span data-stu-id="87cdf-119">isInitial</span></span>|<span data-ttu-id="87cdf-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="87cdf-120">Boolean</span></span>|<span data-ttu-id="87cdf-121">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="87cdf-121">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="87cdf-122">name</span><span class="sxs-lookup"><span data-stu-id="87cdf-122">name</span></span>|<span data-ttu-id="87cdf-123">String</span><span class="sxs-lookup"><span data-stu-id="87cdf-123">String</span></span>|<span data-ttu-id="87cdf-124">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="87cdf-124">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="87cdf-125">type</span><span class="sxs-lookup"><span data-stu-id="87cdf-125">type</span></span>|<span data-ttu-id="87cdf-126">String</span><span class="sxs-lookup"><span data-stu-id="87cdf-126">String</span></span>|<span data-ttu-id="87cdf-127">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="87cdf-127">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87cdf-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87cdf-128">JSON representation</span></span>

<span data-ttu-id="87cdf-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87cdf-129">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
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
