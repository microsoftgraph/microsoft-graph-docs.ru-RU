---
title: Тип ресурса Endpoint
description: 'Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.  Например, при создании новой группы Office 365 дополнительные ресурсы также создаются в составе группы Office 365. Сюда входят такие сведения, как групповой почтовый ящик для бесед и папка OneDrive группы для документов и файлов. Дополнительные сведения об этих ресурсах группы Office 365, в том числе связанные с ними URL-адреса ресурсов, теперь можно прочитать с помощью навигации по *конечным точкам* в типе ресурса Group. Это позволяет приложениям распознавать эти ресурсы и даже внедрять взаимодействие с URL-адресами ресурсов в своих собственных интерфейсах. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 36c69a616cfd1d1aa531f42e9622b4f0c63ec83d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499395"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="98e62-107">Тип ресурса Endpoint</span><span class="sxs-lookup"><span data-stu-id="98e62-107">Endpoint resource type</span></span>

<span data-ttu-id="98e62-108">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="98e62-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98e62-109">Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.</span><span class="sxs-lookup"><span data-stu-id="98e62-109">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="98e62-110">Например, при создании новой группы Office 365 дополнительные ресурсы также создаются в составе группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="98e62-110">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="98e62-111">Сюда входят такие сведения, как групповой почтовый ящик для бесед и папка OneDrive группы для документов и файлов.</span><span class="sxs-lookup"><span data-stu-id="98e62-111">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="98e62-112">Дополнительные сведения об этих ресурсах группы Office 365, в том числе связанные с ними URL-адреса ресурсов, теперь можно прочитать с помощью навигации по *конечным точкам* в типе ресурса Group.</span><span class="sxs-lookup"><span data-stu-id="98e62-112">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="98e62-113">Это позволяет приложениям распознавать эти ресурсы и даже внедрять взаимодействие с URL-адресами ресурсов в своих собственных интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="98e62-113">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="98e62-114">Методы</span><span class="sxs-lookup"><span data-stu-id="98e62-114">Methods</span></span>

| <span data-ttu-id="98e62-115">Метод</span><span class="sxs-lookup"><span data-stu-id="98e62-115">Method</span></span>           | <span data-ttu-id="98e62-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98e62-116">Return Type</span></span>    |<span data-ttu-id="98e62-117">Описание</span><span class="sxs-lookup"><span data-stu-id="98e62-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98e62-118">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="98e62-118">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="98e62-119">Коллекция [Endpoint](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="98e62-119">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="98e62-120">Получение коллекции объектов endpoint.</span><span class="sxs-lookup"><span data-stu-id="98e62-120">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="98e62-121">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="98e62-121">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="98e62-122">Конечная точка</span><span class="sxs-lookup"><span data-stu-id="98e62-122">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="98e62-123">Чтение свойств и связей объекта endpoint.</span><span class="sxs-lookup"><span data-stu-id="98e62-123">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="98e62-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="98e62-124">Properties</span></span>
| <span data-ttu-id="98e62-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="98e62-125">Property</span></span>     | <span data-ttu-id="98e62-126">Тип</span><span class="sxs-lookup"><span data-stu-id="98e62-126">Type</span></span>   |<span data-ttu-id="98e62-127">Описание</span><span class="sxs-lookup"><span data-stu-id="98e62-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="98e62-128">поставлен</span><span class="sxs-lookup"><span data-stu-id="98e62-128">capability</span></span>     | <span data-ttu-id="98e62-129">String</span><span class="sxs-lookup"><span data-stu-id="98e62-129">String</span></span>  | <span data-ttu-id="98e62-130">Описывает возможность, связанную с этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="98e62-130">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="98e62-131">(например, сообщения, беседы и т. д.)  Не допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="98e62-131">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="98e62-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e62-132">Read-only.</span></span> |
| <span data-ttu-id="98e62-133">id</span><span class="sxs-lookup"><span data-stu-id="98e62-133">id</span></span>             | <span data-ttu-id="98e62-134">String</span><span class="sxs-lookup"><span data-stu-id="98e62-134">String</span></span>  | <span data-ttu-id="98e62-135">Уникальный идентификатор для конечной точки; Разделе.</span><span class="sxs-lookup"><span data-stu-id="98e62-135">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="98e62-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="98e62-136">Not nullable.</span></span> <span data-ttu-id="98e62-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e62-137">Read-only.</span></span>|
| <span data-ttu-id="98e62-138">providerId</span><span class="sxs-lookup"><span data-stu-id="98e62-138">providerId</span></span>     | <span data-ttu-id="98e62-139">String</span><span class="sxs-lookup"><span data-stu-id="98e62-139">String</span></span>  | <span data-ttu-id="98e62-140">Идентификатор приложения для базовой службы публикации.</span><span class="sxs-lookup"><span data-stu-id="98e62-140">Application id of the publishing underlying service.</span></span> <span data-ttu-id="98e62-141">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="98e62-141">Not nullable.</span></span> <span data-ttu-id="98e62-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e62-142">Read-only.</span></span>|
| <span data-ttu-id="98e62-143">providerName</span><span class="sxs-lookup"><span data-stu-id="98e62-143">providerName</span></span>   | <span data-ttu-id="98e62-144">String</span><span class="sxs-lookup"><span data-stu-id="98e62-144">String</span></span>  | <span data-ttu-id="98e62-145">Имя базовой службы публикации.</span><span class="sxs-lookup"><span data-stu-id="98e62-145">Name of the publishing underlying service.</span></span> <span data-ttu-id="98e62-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e62-146">Read-only.</span></span>|
| <span data-ttu-id="98e62-147">провидерресаурцеид</span><span class="sxs-lookup"><span data-stu-id="98e62-147">providerResourceId</span></span>|<span data-ttu-id="98e62-148">String</span><span class="sxs-lookup"><span data-stu-id="98e62-148">String</span></span>| <span data-ttu-id="98e62-149">Для групп Office 365 для ресурса задано известное имя ресурса (например, Yammer. Фидурл и т. д.).</span><span class="sxs-lookup"><span data-stu-id="98e62-149">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="98e62-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="98e62-150">Not nullable.</span></span> <span data-ttu-id="98e62-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e62-151">Read-only.</span></span>|
| <span data-ttu-id="98e62-152">URI</span><span class="sxs-lookup"><span data-stu-id="98e62-152">uri</span></span>            | <span data-ttu-id="98e62-153">String</span><span class="sxs-lookup"><span data-stu-id="98e62-153">String</span></span>  | <span data-ttu-id="98e62-154">URL-адрес опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="98e62-154">URL of the published resource.</span></span> <span data-ttu-id="98e62-155">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="98e62-155">Not nullable.</span></span> <span data-ttu-id="98e62-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98e62-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98e62-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="98e62-157">Relationships</span></span>

<span data-ttu-id="98e62-158">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="98e62-158">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="98e62-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98e62-159">JSON representation</span></span>
<span data-ttu-id="98e62-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98e62-160">Here is a JSON representation of the resource.</span></span>

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
