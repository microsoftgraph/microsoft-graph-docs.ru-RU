---
title: Тип ресурса Endpoint
description: Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: yyuank
ms.openlocfilehash: 46c43087ef31537f60a2079e72be71378c140612
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383674"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="960dd-103">Тип ресурса Endpoint</span><span class="sxs-lookup"><span data-stu-id="960dd-103">Endpoint resource type</span></span>

<span data-ttu-id="960dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="960dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="960dd-105">Конечные точки представляют URL-адреса ресурсов, связанных с сущностью.</span><span class="sxs-lookup"><span data-stu-id="960dd-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="960dd-106">Например, при создании новой группы Office 365 дополнительные ресурсы также создаются в составе группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="960dd-106">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="960dd-107">Сюда входят такие сведения, как групповой почтовый ящик для бесед и папка OneDrive группы для документов и файлов.</span><span class="sxs-lookup"><span data-stu-id="960dd-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="960dd-108">Дополнительные сведения об этих ресурсах группы Office 365, в том числе связанные с ними URL-адреса ресурсов, теперь можно прочитать с помощью навигации по *конечным точкам* в типе ресурса Group.</span><span class="sxs-lookup"><span data-stu-id="960dd-108">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="960dd-109">Это позволяет приложениям распознавать эти ресурсы и даже внедрять взаимодействие с URL-адресами ресурсов в своих собственных интерфейсах.</span><span class="sxs-lookup"><span data-stu-id="960dd-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="960dd-110">Методы</span><span class="sxs-lookup"><span data-stu-id="960dd-110">Methods</span></span>

| <span data-ttu-id="960dd-111">Метод</span><span class="sxs-lookup"><span data-stu-id="960dd-111">Method</span></span>           | <span data-ttu-id="960dd-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="960dd-112">Return Type</span></span>    |<span data-ttu-id="960dd-113">Описание</span><span class="sxs-lookup"><span data-stu-id="960dd-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="960dd-114">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="960dd-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="960dd-115">Коллекция [Endpoint](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="960dd-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="960dd-116">Получение коллекции объектов endpoint.</span><span class="sxs-lookup"><span data-stu-id="960dd-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="960dd-117">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="960dd-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="960dd-118">Endpoint</span><span class="sxs-lookup"><span data-stu-id="960dd-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="960dd-119">Чтение свойств и связей объекта endpoint.</span><span class="sxs-lookup"><span data-stu-id="960dd-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="960dd-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="960dd-120">Properties</span></span>
| <span data-ttu-id="960dd-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="960dd-121">Property</span></span>     | <span data-ttu-id="960dd-122">Тип</span><span class="sxs-lookup"><span data-stu-id="960dd-122">Type</span></span>   |<span data-ttu-id="960dd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="960dd-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="960dd-124">поставлен</span><span class="sxs-lookup"><span data-stu-id="960dd-124">capability</span></span>     | <span data-ttu-id="960dd-125">String</span><span class="sxs-lookup"><span data-stu-id="960dd-125">String</span></span>  | <span data-ttu-id="960dd-126">Описывает возможность, связанную с этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="960dd-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="960dd-127">(например, сообщения, беседы и т. д.)  Не допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="960dd-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="960dd-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="960dd-128">Read-only.</span></span> |
| <span data-ttu-id="960dd-129">id</span><span class="sxs-lookup"><span data-stu-id="960dd-129">id</span></span>             | <span data-ttu-id="960dd-130">String</span><span class="sxs-lookup"><span data-stu-id="960dd-130">String</span></span>  | <span data-ttu-id="960dd-131">Уникальный идентификатор для конечной точки; Разделе.</span><span class="sxs-lookup"><span data-stu-id="960dd-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="960dd-132">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="960dd-132">Not nullable.</span></span> <span data-ttu-id="960dd-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="960dd-133">Read-only.</span></span>|
| <span data-ttu-id="960dd-134">providerId</span><span class="sxs-lookup"><span data-stu-id="960dd-134">providerId</span></span>     | <span data-ttu-id="960dd-135">String</span><span class="sxs-lookup"><span data-stu-id="960dd-135">String</span></span>  | <span data-ttu-id="960dd-136">Идентификатор приложения для базовой службы публикации.</span><span class="sxs-lookup"><span data-stu-id="960dd-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="960dd-137">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="960dd-137">Not nullable.</span></span> <span data-ttu-id="960dd-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="960dd-138">Read-only.</span></span>|
| <span data-ttu-id="960dd-139">providerName</span><span class="sxs-lookup"><span data-stu-id="960dd-139">providerName</span></span>   | <span data-ttu-id="960dd-140">String</span><span class="sxs-lookup"><span data-stu-id="960dd-140">String</span></span>  | <span data-ttu-id="960dd-141">Имя базовой службы публикации.</span><span class="sxs-lookup"><span data-stu-id="960dd-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="960dd-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="960dd-142">Read-only.</span></span>|
| <span data-ttu-id="960dd-143">провидерресаурцеид</span><span class="sxs-lookup"><span data-stu-id="960dd-143">providerResourceId</span></span>|<span data-ttu-id="960dd-144">String</span><span class="sxs-lookup"><span data-stu-id="960dd-144">String</span></span>| <span data-ttu-id="960dd-145">Для групп Office 365 для ресурса задано известное имя ресурса (например, Yammer. Фидурл и т. д.).</span><span class="sxs-lookup"><span data-stu-id="960dd-145">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="960dd-146">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="960dd-146">Not nullable.</span></span> <span data-ttu-id="960dd-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="960dd-147">Read-only.</span></span>|
| <span data-ttu-id="960dd-148">URI</span><span class="sxs-lookup"><span data-stu-id="960dd-148">uri</span></span>            | <span data-ttu-id="960dd-149">String</span><span class="sxs-lookup"><span data-stu-id="960dd-149">String</span></span>  | <span data-ttu-id="960dd-150">URL-адрес опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="960dd-150">URL of the published resource.</span></span> <span data-ttu-id="960dd-151">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="960dd-151">Not nullable.</span></span> <span data-ttu-id="960dd-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="960dd-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="960dd-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="960dd-153">Relationships</span></span>

<span data-ttu-id="960dd-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="960dd-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="960dd-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="960dd-155">JSON representation</span></span>
<span data-ttu-id="960dd-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="960dd-156">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
     "Error: microsoft.graph.servicePrincipal/endpoints:\r\n      Referenced type microsoft.graph.endPoint is not defined in the doc  set! Potential suggestion: microsoft.graph.callRecords.endpoint"
    ]
}
-->
