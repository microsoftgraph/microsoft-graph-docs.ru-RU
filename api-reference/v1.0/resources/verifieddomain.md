---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 758d76bd5e1eb577223a41e4e0452179d8bdafc7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033462"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="9126b-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="9126b-104">verifiedDomain resource type</span></span>

<span data-ttu-id="9126b-105">Задает домен клиента.</span><span class="sxs-lookup"><span data-stu-id="9126b-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="9126b-106">Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="9126b-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="9126b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9126b-107">Properties</span></span>
| <span data-ttu-id="9126b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9126b-108">Property</span></span>     | <span data-ttu-id="9126b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9126b-109">Type</span></span>   |<span data-ttu-id="9126b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9126b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9126b-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="9126b-111">capabilities</span></span>|<span data-ttu-id="9126b-112">String</span><span class="sxs-lookup"><span data-stu-id="9126b-112">String</span></span>|<span data-ttu-id="9126b-113">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="9126b-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="9126b-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="9126b-114">isDefault</span></span>|<span data-ttu-id="9126b-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9126b-115">Boolean</span></span>|                <span data-ttu-id="9126b-116">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="9126b-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="9126b-117">при инициализации</span><span class="sxs-lookup"><span data-stu-id="9126b-117">isInitial</span></span>|<span data-ttu-id="9126b-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="9126b-118">Boolean</span></span>|<span data-ttu-id="9126b-119">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="9126b-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="9126b-120">name</span><span class="sxs-lookup"><span data-stu-id="9126b-120">name</span></span>|<span data-ttu-id="9126b-121">String</span><span class="sxs-lookup"><span data-stu-id="9126b-121">String</span></span>|<span data-ttu-id="9126b-122">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="9126b-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="9126b-123">type</span><span class="sxs-lookup"><span data-stu-id="9126b-123">type</span></span>|<span data-ttu-id="9126b-124">String</span><span class="sxs-lookup"><span data-stu-id="9126b-124">String</span></span>|<span data-ttu-id="9126b-125">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="9126b-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9126b-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9126b-126">JSON representation</span></span>

<span data-ttu-id="9126b-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9126b-127">Here is a JSON representation of the resource</span></span>

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
