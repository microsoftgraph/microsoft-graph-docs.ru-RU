---
title: Тип ресурса Принтсервице
description: Представляет специфическое для клиента Azure AD описание экземпляра службы печати. Службы существуют для каждого компонента инфраструктуры печати (например, обнаружение, уведомления, регистрация и протокол IPP) и имеют одну или несколько конечных точек.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fd8641f7fe9fd361e131f0978c8f677a6395e405
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896071"
---
# <a name="printservice-resource-type"></a><span data-ttu-id="105db-104">Тип ресурса Принтсервице</span><span class="sxs-lookup"><span data-stu-id="105db-104">printService resource type</span></span>

<span data-ttu-id="105db-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="105db-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="105db-106">Представляет специфическое для клиента Azure AD описание экземпляра службы печати.</span><span class="sxs-lookup"><span data-stu-id="105db-106">Represents an Azure AD tenant-specific description of a print service instance.</span></span> <span data-ttu-id="105db-107">Службы существуют для каждого компонента инфраструктуры печати (обнаружение, уведомления, регистрация и протокол IPP) и имеют одну или несколько конечных точек.</span><span class="sxs-lookup"><span data-stu-id="105db-107">Services exist for each component of the printing infrastructure (discovery, notifications, registration, and IPP) and have one or more endpoints.</span></span>

## <a name="methods"></a><span data-ttu-id="105db-108">Методы</span><span class="sxs-lookup"><span data-stu-id="105db-108">Methods</span></span>

| <span data-ttu-id="105db-109">Метод</span><span class="sxs-lookup"><span data-stu-id="105db-109">Method</span></span>       | <span data-ttu-id="105db-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="105db-110">Return Type</span></span> | <span data-ttu-id="105db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="105db-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="105db-112">Список служб</span><span class="sxs-lookup"><span data-stu-id="105db-112">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="105db-113">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="105db-113">[printService](printservice.md) collection</span></span> | <span data-ttu-id="105db-114">Получение списка универсальных служб печати.</span><span class="sxs-lookup"><span data-stu-id="105db-114">Get a list of Universal Print services.</span></span> |
| [<span data-ttu-id="105db-115">Получение службы</span><span class="sxs-lookup"><span data-stu-id="105db-115">Get service</span></span>](../api/printservice-get.md) | [<span data-ttu-id="105db-116">принтсервице</span><span class="sxs-lookup"><span data-stu-id="105db-116">printService</span></span>](printservice.md) | <span data-ttu-id="105db-117">Считывание свойств и связей объекта Service.</span><span class="sxs-lookup"><span data-stu-id="105db-117">Read the properties and relationships of service object.</span></span> |
| [<span data-ttu-id="105db-118">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="105db-118">List endpoints</span></span>](../api/printservice-list-endpoints.md) | <span data-ttu-id="105db-119">Коллекция [принтсервицеендпоинт](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="105db-119">[printServiceEndpoint](printserviceendpoint.md) collection</span></span> | <span data-ttu-id="105db-120">Получение списка конечных точек, предоставляемых службой.</span><span class="sxs-lookup"><span data-stu-id="105db-120">Get a list of endpoints that a service provides.</span></span> |

## <a name="properties"></a><span data-ttu-id="105db-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="105db-121">Properties</span></span>
| <span data-ttu-id="105db-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="105db-122">Property</span></span>     | <span data-ttu-id="105db-123">Тип</span><span class="sxs-lookup"><span data-stu-id="105db-123">Type</span></span>        | <span data-ttu-id="105db-124">Описание</span><span class="sxs-lookup"><span data-stu-id="105db-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="105db-125">id</span><span class="sxs-lookup"><span data-stu-id="105db-125">id</span></span>|<span data-ttu-id="105db-126">String</span><span class="sxs-lookup"><span data-stu-id="105db-126">String</span></span>|<span data-ttu-id="105db-127">Идентификатор службы.</span><span class="sxs-lookup"><span data-stu-id="105db-127">The service's identifier.</span></span> <span data-ttu-id="105db-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="105db-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="105db-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="105db-129">Relationships</span></span>
| <span data-ttu-id="105db-130">Связь</span><span class="sxs-lookup"><span data-stu-id="105db-130">Relationship</span></span> | <span data-ttu-id="105db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="105db-131">Type</span></span>        | <span data-ttu-id="105db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="105db-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="105db-133">endpoints</span><span class="sxs-lookup"><span data-stu-id="105db-133">endpoints</span></span>|<span data-ttu-id="105db-134">Коллекция [принтсервицеендпоинт](printserviceendpoint.md)</span><span class="sxs-lookup"><span data-stu-id="105db-134">[printServiceEndpoint](printserviceendpoint.md) collection</span></span>| <span data-ttu-id="105db-135">Конечные точки, которые можно использовать для доступа к службе.</span><span class="sxs-lookup"><span data-stu-id="105db-135">Endpoints that can be used to access the service.</span></span> <span data-ttu-id="105db-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="105db-136">Read-only.</span></span> <span data-ttu-id="105db-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="105db-137">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="105db-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="105db-138">JSON representation</span></span>

<span data-ttu-id="105db-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="105db-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printService",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "endpoints": [ {"@odata.type": "microsoft.graph.printServiceEndpoint"} ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->