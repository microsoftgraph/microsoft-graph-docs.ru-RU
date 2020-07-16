---
title: Тип ресурса Endpoint
description: 'Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.  Например, при создании новой группы Microsoft 365 дополнительные ресурсы также создаются как часть группы Microsoft 365. Сюда входят такие сведения, как групповой почтовый ящик для бесед и папка OneDrive группы для документов и файлов. Дополнительные сведения об этих ресурсах группы Microsoft 365, в том числе связанные с ними URL-адреса ресурсов, теперь можно прочитать с помощью навигации по *конечным точкам* в типе ресурса Group. Это позволяет приложениям распознавать эти ресурсы и даже внедрять взаимодействие с URL-адресами ресурсов в своих собственных интерфейсах. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 77a0ddc0a91f1269ed5e62393c32b85af49264aa
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44893853"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="0a73b-107">Тип ресурса Endpoint</span><span class="sxs-lookup"><span data-stu-id="0a73b-107">Endpoint resource type</span></span>

<span data-ttu-id="0a73b-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a73b-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a73b-109">Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.</span><span class="sxs-lookup"><span data-stu-id="0a73b-109">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="0a73b-110">Например, при создании новой группы Microsoft 365 дополнительные ресурсы также создаются как часть группы Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0a73b-110">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="0a73b-111">Сюда входят такие сведения, как групповой почтовый ящик для бесед и папка OneDrive группы для документов и файлов.</span><span class="sxs-lookup"><span data-stu-id="0a73b-111">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="0a73b-112">Дополнительные сведения об этих ресурсах группы Microsoft 365, в том числе связанные с ними URL-адреса ресурсов, теперь можно прочитать с помощью навигации по *конечным точкам* в типе ресурса Group.</span><span class="sxs-lookup"><span data-stu-id="0a73b-112">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="0a73b-113">Это позволяет приложениям распознавать эти ресурсы и даже внедрять взаимодействие с URL-адресами ресурсов в своих собственных интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="0a73b-113">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="0a73b-114">Методы</span><span class="sxs-lookup"><span data-stu-id="0a73b-114">Methods</span></span>

| <span data-ttu-id="0a73b-115">Метод</span><span class="sxs-lookup"><span data-stu-id="0a73b-115">Method</span></span>           | <span data-ttu-id="0a73b-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0a73b-116">Return Type</span></span>    |<span data-ttu-id="0a73b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="0a73b-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a73b-118">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="0a73b-118">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="0a73b-119">Коллекция [Endpoint](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="0a73b-119">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="0a73b-120">Получение коллекции объектов endpoint.</span><span class="sxs-lookup"><span data-stu-id="0a73b-120">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="0a73b-121">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="0a73b-121">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="0a73b-122">Конечная точка</span><span class="sxs-lookup"><span data-stu-id="0a73b-122">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="0a73b-123">Чтение свойств и связей объекта endpoint.</span><span class="sxs-lookup"><span data-stu-id="0a73b-123">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0a73b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a73b-124">Properties</span></span>
| <span data-ttu-id="0a73b-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a73b-125">Property</span></span>     | <span data-ttu-id="0a73b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="0a73b-126">Type</span></span>   |<span data-ttu-id="0a73b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="0a73b-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0a73b-128">поставлен</span><span class="sxs-lookup"><span data-stu-id="0a73b-128">capability</span></span>     | <span data-ttu-id="0a73b-129">String</span><span class="sxs-lookup"><span data-stu-id="0a73b-129">String</span></span>  | <span data-ttu-id="0a73b-130">Описывает возможность, связанную с этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="0a73b-130">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="0a73b-131">(например, сообщения, беседы и т. д.)  Не допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="0a73b-131">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="0a73b-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a73b-132">Read-only.</span></span> |
| <span data-ttu-id="0a73b-133">id</span><span class="sxs-lookup"><span data-stu-id="0a73b-133">id</span></span>             | <span data-ttu-id="0a73b-134">String</span><span class="sxs-lookup"><span data-stu-id="0a73b-134">String</span></span>  | <span data-ttu-id="0a73b-135">Уникальный идентификатор для конечной точки; Разделе.</span><span class="sxs-lookup"><span data-stu-id="0a73b-135">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="0a73b-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0a73b-136">Not nullable.</span></span> <span data-ttu-id="0a73b-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a73b-137">Read-only.</span></span>|
| <span data-ttu-id="0a73b-138">providerId</span><span class="sxs-lookup"><span data-stu-id="0a73b-138">providerId</span></span>     | <span data-ttu-id="0a73b-139">String</span><span class="sxs-lookup"><span data-stu-id="0a73b-139">String</span></span>  | <span data-ttu-id="0a73b-140">Идентификатор приложения для базовой службы публикации.</span><span class="sxs-lookup"><span data-stu-id="0a73b-140">Application id of the publishing underlying service.</span></span> <span data-ttu-id="0a73b-141">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0a73b-141">Not nullable.</span></span> <span data-ttu-id="0a73b-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a73b-142">Read-only.</span></span>|
| <span data-ttu-id="0a73b-143">providerName</span><span class="sxs-lookup"><span data-stu-id="0a73b-143">providerName</span></span>   | <span data-ttu-id="0a73b-144">String</span><span class="sxs-lookup"><span data-stu-id="0a73b-144">String</span></span>  | <span data-ttu-id="0a73b-145">Имя базовой службы публикации.</span><span class="sxs-lookup"><span data-stu-id="0a73b-145">Name of the publishing underlying service.</span></span> <span data-ttu-id="0a73b-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a73b-146">Read-only.</span></span>|
| <span data-ttu-id="0a73b-147">провидерресаурцеид</span><span class="sxs-lookup"><span data-stu-id="0a73b-147">providerResourceId</span></span>|<span data-ttu-id="0a73b-148">String</span><span class="sxs-lookup"><span data-stu-id="0a73b-148">String</span></span>| <span data-ttu-id="0a73b-149">Для групп Microsoft 365 для ресурса задано известное имя ресурса (например, Yammer. Фидурл и т. д.).</span><span class="sxs-lookup"><span data-stu-id="0a73b-149">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="0a73b-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0a73b-150">Not nullable.</span></span> <span data-ttu-id="0a73b-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a73b-151">Read-only.</span></span>|
| <span data-ttu-id="0a73b-152">URI</span><span class="sxs-lookup"><span data-stu-id="0a73b-152">uri</span></span>            | <span data-ttu-id="0a73b-153">String</span><span class="sxs-lookup"><span data-stu-id="0a73b-153">String</span></span>  | <span data-ttu-id="0a73b-154">URL-адрес опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="0a73b-154">URL of the published resource.</span></span> <span data-ttu-id="0a73b-155">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0a73b-155">Not nullable.</span></span> <span data-ttu-id="0a73b-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a73b-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a73b-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="0a73b-157">Relationships</span></span>

<span data-ttu-id="0a73b-158">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0a73b-158">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0a73b-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0a73b-159">JSON representation</span></span>
<span data-ttu-id="0a73b-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a73b-160">Here is a JSON representation of the resource.</span></span>

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
