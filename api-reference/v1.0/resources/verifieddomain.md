---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
author: davidmu1
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e2d26cd5e74499b5f2a086dfaa0ca9e9cbf4a4d8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135550"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="0a3da-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="0a3da-104">verifiedDomain resource type</span></span>

<span data-ttu-id="0a3da-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a3da-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a3da-106">Задает домен клиента.</span><span class="sxs-lookup"><span data-stu-id="0a3da-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="0a3da-107">Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="0a3da-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="0a3da-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a3da-108">Properties</span></span>
| <span data-ttu-id="0a3da-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a3da-109">Property</span></span>     | <span data-ttu-id="0a3da-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0a3da-110">Type</span></span>   |<span data-ttu-id="0a3da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a3da-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a3da-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="0a3da-112">capabilities</span></span>|<span data-ttu-id="0a3da-113">String</span><span class="sxs-lookup"><span data-stu-id="0a3da-113">String</span></span>|<span data-ttu-id="0a3da-114">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="0a3da-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="0a3da-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="0a3da-115">isDefault</span></span>|<span data-ttu-id="0a3da-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a3da-116">Boolean</span></span>|                <span data-ttu-id="0a3da-117">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="0a3da-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="0a3da-118">isInitial</span><span class="sxs-lookup"><span data-stu-id="0a3da-118">isInitial</span></span>|<span data-ttu-id="0a3da-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a3da-119">Boolean</span></span>|<span data-ttu-id="0a3da-120">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="0a3da-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="0a3da-121">name</span><span class="sxs-lookup"><span data-stu-id="0a3da-121">name</span></span>|<span data-ttu-id="0a3da-122">String</span><span class="sxs-lookup"><span data-stu-id="0a3da-122">String</span></span>|<span data-ttu-id="0a3da-123">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="0a3da-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="0a3da-124">type</span><span class="sxs-lookup"><span data-stu-id="0a3da-124">type</span></span>|<span data-ttu-id="0a3da-125">String</span><span class="sxs-lookup"><span data-stu-id="0a3da-125">String</span></span>|<span data-ttu-id="0a3da-126">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="0a3da-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a3da-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a3da-127">JSON representation</span></span>

<span data-ttu-id="0a3da-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a3da-128">Here is a JSON representation of the resource</span></span>

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

