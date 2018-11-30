---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
ms.openlocfilehash: 21b6dd89dcc8b990046952d9ae7abcfe8ce02bca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025757"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="84528-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="84528-104">verifiedDomain resource type</span></span>

<span data-ttu-id="84528-p102">Задает домен клиента. Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="84528-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="84528-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="84528-107">Properties</span></span>
| <span data-ttu-id="84528-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="84528-108">Property</span></span>     | <span data-ttu-id="84528-109">Тип</span><span class="sxs-lookup"><span data-stu-id="84528-109">Type</span></span>   |<span data-ttu-id="84528-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84528-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84528-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="84528-111">capabilities</span></span>|<span data-ttu-id="84528-112">String</span><span class="sxs-lookup"><span data-stu-id="84528-112">String</span></span>|<span data-ttu-id="84528-113">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="84528-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="84528-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="84528-114">isDefault</span></span>|<span data-ttu-id="84528-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="84528-115">Boolean</span></span>|                <span data-ttu-id="84528-116">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="84528-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="84528-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="84528-117">isInitial</span></span>|<span data-ttu-id="84528-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="84528-118">Boolean</span></span>|<span data-ttu-id="84528-119">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="84528-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="84528-120">name</span><span class="sxs-lookup"><span data-stu-id="84528-120">name</span></span>|<span data-ttu-id="84528-121">String</span><span class="sxs-lookup"><span data-stu-id="84528-121">String</span></span>|<span data-ttu-id="84528-122">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="84528-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="84528-123">type</span><span class="sxs-lookup"><span data-stu-id="84528-123">type</span></span>|<span data-ttu-id="84528-124">String</span><span class="sxs-lookup"><span data-stu-id="84528-124">String</span></span>|<span data-ttu-id="84528-125">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="84528-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84528-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84528-126">JSON representation</span></span>

<span data-ttu-id="84528-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84528-127">Here is a JSON representation of the resource</span></span>

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
