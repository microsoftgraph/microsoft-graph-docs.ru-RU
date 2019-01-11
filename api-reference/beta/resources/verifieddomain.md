---
title: Тип ресурса verifiedDomain
description: Задает домен клиента. Свойство **verifiedDomains** объекта organization представляет собой коллекцию объектов **VerifiedDomain**.
localization_priority: Normal
ms.openlocfilehash: d912103f95677491d88bcb3f0b556bb1678c3049
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810446"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="c2d84-104">Тип ресурса verifiedDomain</span><span class="sxs-lookup"><span data-stu-id="c2d84-104">verifiedDomain resource type</span></span>

> <span data-ttu-id="c2d84-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2d84-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2d84-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d84-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2d84-p103">Задает домен клиента. Свойство **verifiedDomains** объекта [organization](organization.md) представляет собой коллекцию объектов **VerifiedDomain**.</span><span class="sxs-lookup"><span data-stu-id="c2d84-p103">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="c2d84-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2d84-109">Properties</span></span>
| <span data-ttu-id="c2d84-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d84-110">Property</span></span>     | <span data-ttu-id="c2d84-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d84-111">Type</span></span>   |<span data-ttu-id="c2d84-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d84-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2d84-113">capabilities</span><span class="sxs-lookup"><span data-stu-id="c2d84-113">capabilities</span></span>|<span data-ttu-id="c2d84-114">String</span><span class="sxs-lookup"><span data-stu-id="c2d84-114">String</span></span>|<span data-ttu-id="c2d84-115">Примеры: “Email”, “OfficeCommunicationsOnline”.</span><span class="sxs-lookup"><span data-stu-id="c2d84-115">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="c2d84-116">isDefault</span><span class="sxs-lookup"><span data-stu-id="c2d84-116">isDefault</span></span>|<span data-ttu-id="c2d84-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2d84-117">Boolean</span></span>|                <span data-ttu-id="c2d84-118">Значение **true** указывает, что это связанный с клиентом домен по умолчанию. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="c2d84-118">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="c2d84-119">isInitial</span><span class="sxs-lookup"><span data-stu-id="c2d84-119">isInitial</span></span>|<span data-ttu-id="c2d84-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2d84-120">Boolean</span></span>|<span data-ttu-id="c2d84-121">Значение **true** указывает, что это первоначальный домен, связанный с клиентом. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="c2d84-121">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="c2d84-122">name</span><span class="sxs-lookup"><span data-stu-id="c2d84-122">name</span></span>|<span data-ttu-id="c2d84-123">String</span><span class="sxs-lookup"><span data-stu-id="c2d84-123">String</span></span>|<span data-ttu-id="c2d84-124">Доменное имя, например "contoso.onmicrosoft.com"</span><span class="sxs-lookup"><span data-stu-id="c2d84-124">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="c2d84-125">type</span><span class="sxs-lookup"><span data-stu-id="c2d84-125">type</span></span>|<span data-ttu-id="c2d84-126">String</span><span class="sxs-lookup"><span data-stu-id="c2d84-126">String</span></span>|<span data-ttu-id="c2d84-127">Пример: "Managed".</span><span class="sxs-lookup"><span data-stu-id="c2d84-127">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2d84-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2d84-128">JSON representation</span></span>

<span data-ttu-id="c2d84-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2d84-129">Here is a JSON representation of the resource</span></span>

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
