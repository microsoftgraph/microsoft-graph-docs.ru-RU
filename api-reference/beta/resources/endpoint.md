---
title: Тип ресурса конечной точки
description: Конечные точки представляют URL-адреса для ресурсов, связанных с объектом.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: groups
author: Jordanndahl
ms.openlocfilehash: 1b5c9f401a659f1461cb9c2185dd412154dbeeda
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680411"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="25555-103">Тип ресурса конечной точки</span><span class="sxs-lookup"><span data-stu-id="25555-103">Endpoint resource type</span></span>

<span data-ttu-id="25555-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25555-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25555-105">Конечные точки представляют URL-адреса для ресурсов, связанных с объектом.</span><span class="sxs-lookup"><span data-stu-id="25555-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="25555-106">Например, при Microsoft 365 группы создаются дополнительные ресурсы в составе Microsoft 365 группы.</span><span class="sxs-lookup"><span data-stu-id="25555-106">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="25555-107">К ним относятся такие вещи, как групповой почтовый ящик для бесед и OneDrive папка для документов и файлов.</span><span class="sxs-lookup"><span data-stu-id="25555-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="25555-108">Дополнительные сведения об этих Microsoft 365, включая связанные с ними URL-адреса  ресурсов, теперь можно прочитать с помощью навигации конечных точек на типе ресурсов группы.</span><span class="sxs-lookup"><span data-stu-id="25555-108">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="25555-109">Это позволяет приложениям понимать эти ресурсы и даже встраить url-адреса ресурсов в свои собственные возможности.</span><span class="sxs-lookup"><span data-stu-id="25555-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span>

## <a name="methods"></a><span data-ttu-id="25555-110">Методы</span><span class="sxs-lookup"><span data-stu-id="25555-110">Methods</span></span>

| <span data-ttu-id="25555-111">Метод</span><span class="sxs-lookup"><span data-stu-id="25555-111">Method</span></span>           | <span data-ttu-id="25555-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="25555-112">Return Type</span></span>    |<span data-ttu-id="25555-113">Описание</span><span class="sxs-lookup"><span data-stu-id="25555-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25555-114">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="25555-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="25555-115">Коллекция [Endpoint](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="25555-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="25555-116">Получение коллекции объектов endpoint.</span><span class="sxs-lookup"><span data-stu-id="25555-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="25555-117">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="25555-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="25555-118">Конечная точка</span><span class="sxs-lookup"><span data-stu-id="25555-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="25555-119">Чтение свойств и связей объекта endpoint.</span><span class="sxs-lookup"><span data-stu-id="25555-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="25555-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="25555-120">Properties</span></span>
| <span data-ttu-id="25555-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="25555-121">Property</span></span>     | <span data-ttu-id="25555-122">Тип</span><span class="sxs-lookup"><span data-stu-id="25555-122">Type</span></span>   |<span data-ttu-id="25555-123">Описание</span><span class="sxs-lookup"><span data-stu-id="25555-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25555-124">возможности</span><span class="sxs-lookup"><span data-stu-id="25555-124">capability</span></span>     | <span data-ttu-id="25555-125">String</span><span class="sxs-lookup"><span data-stu-id="25555-125">String</span></span>  | <span data-ttu-id="25555-126">Описывает возможности, связанные с этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="25555-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="25555-127">(например, сообщения, беседы и т.д.)  Не является nullable.</span><span class="sxs-lookup"><span data-stu-id="25555-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="25555-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25555-128">Read-only.</span></span> |
| <span data-ttu-id="25555-129">id</span><span class="sxs-lookup"><span data-stu-id="25555-129">id</span></span>             | <span data-ttu-id="25555-130">String</span><span class="sxs-lookup"><span data-stu-id="25555-130">String</span></span>  | <span data-ttu-id="25555-131">Уникальный идентификатор конечной точки; Ключ.</span><span class="sxs-lookup"><span data-stu-id="25555-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="25555-132">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="25555-132">Not nullable.</span></span> <span data-ttu-id="25555-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25555-133">Read-only.</span></span>|
| <span data-ttu-id="25555-134">providerId</span><span class="sxs-lookup"><span data-stu-id="25555-134">providerId</span></span>     | <span data-ttu-id="25555-135">String</span><span class="sxs-lookup"><span data-stu-id="25555-135">String</span></span>  | <span data-ttu-id="25555-136">ID приложения службы публикации.</span><span class="sxs-lookup"><span data-stu-id="25555-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="25555-137">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="25555-137">Not nullable.</span></span> <span data-ttu-id="25555-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25555-138">Read-only.</span></span>|
| <span data-ttu-id="25555-139">providerName</span><span class="sxs-lookup"><span data-stu-id="25555-139">providerName</span></span>   | <span data-ttu-id="25555-140">String</span><span class="sxs-lookup"><span data-stu-id="25555-140">String</span></span>  | <span data-ttu-id="25555-141">Имя службы публикации.</span><span class="sxs-lookup"><span data-stu-id="25555-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="25555-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25555-142">Read-only.</span></span>|
| <span data-ttu-id="25555-143">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="25555-143">providerResourceId</span></span>|<span data-ttu-id="25555-144">String</span><span class="sxs-lookup"><span data-stu-id="25555-144">String</span></span>| <span data-ttu-id="25555-145">Для Microsoft 365 групп это имя для ресурса (например, Yammer. FeedURL и т.д.).</span><span class="sxs-lookup"><span data-stu-id="25555-145">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="25555-146">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="25555-146">Not nullable.</span></span> <span data-ttu-id="25555-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25555-147">Read-only.</span></span>|
| <span data-ttu-id="25555-148">uri</span><span class="sxs-lookup"><span data-stu-id="25555-148">uri</span></span>            | <span data-ttu-id="25555-149">String</span><span class="sxs-lookup"><span data-stu-id="25555-149">String</span></span>  | <span data-ttu-id="25555-150">URL-адрес опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="25555-150">URL of the published resource.</span></span> <span data-ttu-id="25555-151">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="25555-151">Not nullable.</span></span> <span data-ttu-id="25555-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25555-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25555-153">Связи</span><span class="sxs-lookup"><span data-stu-id="25555-153">Relationships</span></span>

<span data-ttu-id="25555-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25555-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="25555-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25555-155">JSON representation</span></span>
<span data-ttu-id="25555-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25555-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


