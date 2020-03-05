---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 20766f236bc3f9d8702a257fa3073a4fa205ce51
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446774"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="aa61a-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="aa61a-104">verifiedDomain resource type</span></span>

<span data-ttu-id="aa61a-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aa61a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa61a-106">Задает домен клиента.</span><span class="sxs-lookup"><span data-stu-id="aa61a-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="aa61a-107">Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="aa61a-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="aa61a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa61a-108">Properties</span></span>
| <span data-ttu-id="aa61a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa61a-109">Property</span></span>     | <span data-ttu-id="aa61a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aa61a-110">Type</span></span>   |<span data-ttu-id="aa61a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aa61a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa61a-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="aa61a-112">capabilities</span></span>|<span data-ttu-id="aa61a-113">String</span><span class="sxs-lookup"><span data-stu-id="aa61a-113">String</span></span>|<span data-ttu-id="aa61a-114">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="aa61a-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="aa61a-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="aa61a-115">isDefault</span></span>|<span data-ttu-id="aa61a-116">Логический</span><span class="sxs-lookup"><span data-stu-id="aa61a-116">Boolean</span></span>|                <span data-ttu-id="aa61a-117">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="aa61a-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="aa61a-118">при инициализации</span><span class="sxs-lookup"><span data-stu-id="aa61a-118">isInitial</span></span>|<span data-ttu-id="aa61a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa61a-119">Boolean</span></span>|<span data-ttu-id="aa61a-120">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="aa61a-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="aa61a-121">name</span><span class="sxs-lookup"><span data-stu-id="aa61a-121">name</span></span>|<span data-ttu-id="aa61a-122">String</span><span class="sxs-lookup"><span data-stu-id="aa61a-122">String</span></span>|<span data-ttu-id="aa61a-123">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="aa61a-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="aa61a-124">type</span><span class="sxs-lookup"><span data-stu-id="aa61a-124">type</span></span>|<span data-ttu-id="aa61a-125">String</span><span class="sxs-lookup"><span data-stu-id="aa61a-125">String</span></span>|<span data-ttu-id="aa61a-126">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="aa61a-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa61a-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa61a-127">JSON representation</span></span>

<span data-ttu-id="aa61a-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa61a-128">Here is a JSON representation of the resource</span></span>

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
