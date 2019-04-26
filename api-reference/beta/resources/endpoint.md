---
title: Тип ресурса Endpoint
description: 'Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.  Например, при создании новой группы Office 365 дополнительные ресурсы также создаются в составе группы Office 365. Сюда входят такие сведения, как групповой почтовый ящик для бесед и папка OneDrive группы для документов и файлов. Дополнительные сведения об этих ресурсах группы Office 365, в том числе связанные с ними URL-адреса ресурсов ** , теперь можно прочитать с помощью навигации по конечным точкам в типе ресурса Group. Это позволяет приложениям распознавать эти ресурсы и даже внедрять взаимодействие с URL-АДРЕСами ресурсов в своих собственных интерфейсах. '
localization_priority: Normal
ms.openlocfilehash: 474da77d10d9b433dd6d4914f9b75812e040a9e4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340213"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="84716-107">Тип ресурса Endpoint</span><span class="sxs-lookup"><span data-stu-id="84716-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84716-108">Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.</span><span class="sxs-lookup"><span data-stu-id="84716-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="84716-109">Например, при создании новой группы Office 365 дополнительные ресурсы также создаются в составе группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="84716-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="84716-110">Сюда входят такие сведения, как групповой почтовый ящик для бесед и папка OneDrive группы для документов и файлов.</span><span class="sxs-lookup"><span data-stu-id="84716-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="84716-111">Дополнительные сведения об этих ресурсах группы Office 365, в том числе связанные с ними URL-адреса ресурсов \*\* , теперь можно прочитать с помощью навигации по конечным точкам в типе ресурса Group.</span><span class="sxs-lookup"><span data-stu-id="84716-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="84716-112">Это позволяет приложениям распознавать эти ресурсы и даже внедрять взаимодействие с URL-АДРЕСами ресурсов в своих собственных интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="84716-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="84716-113">Методы</span><span class="sxs-lookup"><span data-stu-id="84716-113">Methods</span></span>

| <span data-ttu-id="84716-114">Метод</span><span class="sxs-lookup"><span data-stu-id="84716-114">Method</span></span>           | <span data-ttu-id="84716-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="84716-115">Return Type</span></span>    |<span data-ttu-id="84716-116">Описание</span><span class="sxs-lookup"><span data-stu-id="84716-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84716-117">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="84716-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="84716-118">Коллекция [Endpoint](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="84716-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="84716-119">Получение коллекции объектов endpoint.</span><span class="sxs-lookup"><span data-stu-id="84716-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="84716-120">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="84716-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="84716-121">Конечная точка</span><span class="sxs-lookup"><span data-stu-id="84716-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="84716-122">Чтение свойств и связей объекта endpoint.</span><span class="sxs-lookup"><span data-stu-id="84716-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84716-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="84716-123">Properties</span></span>
| <span data-ttu-id="84716-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="84716-124">Property</span></span>     | <span data-ttu-id="84716-125">Тип</span><span class="sxs-lookup"><span data-stu-id="84716-125">Type</span></span>   |<span data-ttu-id="84716-126">Описание</span><span class="sxs-lookup"><span data-stu-id="84716-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="84716-127">поставлен</span><span class="sxs-lookup"><span data-stu-id="84716-127">capability</span></span>     | <span data-ttu-id="84716-128">String</span><span class="sxs-lookup"><span data-stu-id="84716-128">String</span></span>  | <span data-ttu-id="84716-129">Описывает возможность, связанную с этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="84716-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="84716-130">(например, сообщения, беседы и т. д.)  Не допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="84716-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="84716-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84716-131">Read-only.</span></span> |
| <span data-ttu-id="84716-132">id</span><span class="sxs-lookup"><span data-stu-id="84716-132">id</span></span>             | <span data-ttu-id="84716-133">String</span><span class="sxs-lookup"><span data-stu-id="84716-133">String</span></span>  | <span data-ttu-id="84716-134">Уникальный идентификатор для конечной точки; Разделе.</span><span class="sxs-lookup"><span data-stu-id="84716-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="84716-135">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="84716-135">Not nullable.</span></span> <span data-ttu-id="84716-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84716-136">Read-only.</span></span>|
| <span data-ttu-id="84716-137">providerId</span><span class="sxs-lookup"><span data-stu-id="84716-137">providerId</span></span>     | <span data-ttu-id="84716-138">String</span><span class="sxs-lookup"><span data-stu-id="84716-138">String</span></span>  | <span data-ttu-id="84716-139">Идентификатор приложения для базовой службы публикации.</span><span class="sxs-lookup"><span data-stu-id="84716-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="84716-140">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="84716-140">Not nullable.</span></span> <span data-ttu-id="84716-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84716-141">Read-only.</span></span>|
| <span data-ttu-id="84716-142">providerName</span><span class="sxs-lookup"><span data-stu-id="84716-142">providerName</span></span>   | <span data-ttu-id="84716-143">String</span><span class="sxs-lookup"><span data-stu-id="84716-143">String</span></span>  | <span data-ttu-id="84716-144">Имя базовой службы публикации.</span><span class="sxs-lookup"><span data-stu-id="84716-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="84716-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84716-145">Read-only.</span></span>|
| <span data-ttu-id="84716-146">Провидерресаурцеид</span><span class="sxs-lookup"><span data-stu-id="84716-146">providerResourceId</span></span>|<span data-ttu-id="84716-147">String</span><span class="sxs-lookup"><span data-stu-id="84716-147">String</span></span>| <span data-ttu-id="84716-148">Для групп Office 365 для ресурса задано известное имя ресурса (например, Yammer. Фидурл и т. д.).</span><span class="sxs-lookup"><span data-stu-id="84716-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="84716-149">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="84716-149">Not nullable.</span></span> <span data-ttu-id="84716-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84716-150">Read-only.</span></span>|
| <span data-ttu-id="84716-151">URI</span><span class="sxs-lookup"><span data-stu-id="84716-151">uri</span></span>            | <span data-ttu-id="84716-152">String</span><span class="sxs-lookup"><span data-stu-id="84716-152">String</span></span>  | <span data-ttu-id="84716-153">URL-адрес опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="84716-153">URL of the published resource.</span></span> <span data-ttu-id="84716-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="84716-154">Not nullable.</span></span> <span data-ttu-id="84716-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84716-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84716-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="84716-156">Relationships</span></span>

<span data-ttu-id="84716-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84716-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="84716-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="84716-158">JSON representation</span></span>
<span data-ttu-id="84716-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84716-159">Here is a JSON representation of the resource.</span></span>

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
