---
title: Тип ресурса Endpoint
description: Конечные точки представляют URL-адреса для ресурсов, связанных с сущностью.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: yyuank
ms.openlocfilehash: 47bef2bfa14fb8a00fd1ca2356d7f880ff3207d6
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013606"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="8debc-103">Тип ресурса Endpoint</span><span class="sxs-lookup"><span data-stu-id="8debc-103">Endpoint resource type</span></span>

<span data-ttu-id="8debc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8debc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8debc-105">Конечные точки представляют URL-адреса для ресурсов, связанных с сущностью.</span><span class="sxs-lookup"><span data-stu-id="8debc-105">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="8debc-106">Например, при создании новой группы Microsoft 365 в составе группы Microsoft 365 также создаются дополнительные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="8debc-106">For example, when a new Microsoft 365 group is created, additional resources are also created as part of the Microsoft 365 group.</span></span> <span data-ttu-id="8debc-107">К ним относятся почтовый ящик группы для бесед и папка группы OneDrive для документов и файлов.</span><span class="sxs-lookup"><span data-stu-id="8debc-107">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="8debc-108">Дополнительные сведения об этих ресурсах группы Microsoft 365, включая связанные  с ними URL-адреса ресурсов, теперь можно читать с помощью навигации конечных точек на типе ресурса группы.</span><span class="sxs-lookup"><span data-stu-id="8debc-108">Further information about these Microsoft 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="8debc-109">Это позволяет приложениям понять эти ресурсы и даже встраить возможности ИСПОЛЬЗОВАНИЯ URL-адресов ресурсов в собственные возможности.</span><span class="sxs-lookup"><span data-stu-id="8debc-109">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span>

## <a name="methods"></a><span data-ttu-id="8debc-110">Методы</span><span class="sxs-lookup"><span data-stu-id="8debc-110">Methods</span></span>

| <span data-ttu-id="8debc-111">Метод</span><span class="sxs-lookup"><span data-stu-id="8debc-111">Method</span></span>           | <span data-ttu-id="8debc-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8debc-112">Return Type</span></span>    |<span data-ttu-id="8debc-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8debc-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8debc-114">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="8debc-114">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="8debc-115">Коллекция [Endpoint](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="8debc-115">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="8debc-116">Получение коллекции объектов endpoint.</span><span class="sxs-lookup"><span data-stu-id="8debc-116">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="8debc-117">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="8debc-117">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="8debc-118">Конечная точка</span><span class="sxs-lookup"><span data-stu-id="8debc-118">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="8debc-119">Чтение свойств и связей объекта endpoint.</span><span class="sxs-lookup"><span data-stu-id="8debc-119">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8debc-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="8debc-120">Properties</span></span>
| <span data-ttu-id="8debc-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="8debc-121">Property</span></span>     | <span data-ttu-id="8debc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8debc-122">Type</span></span>   |<span data-ttu-id="8debc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8debc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8debc-124">capability</span><span class="sxs-lookup"><span data-stu-id="8debc-124">capability</span></span>     | <span data-ttu-id="8debc-125">String</span><span class="sxs-lookup"><span data-stu-id="8debc-125">String</span></span>  | <span data-ttu-id="8debc-126">Описание возможности, связанной с этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="8debc-126">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="8debc-127">(Например, сообщения, беседы и т. д.)  Не имеет null.</span><span class="sxs-lookup"><span data-stu-id="8debc-127">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="8debc-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8debc-128">Read-only.</span></span> |
| <span data-ttu-id="8debc-129">id</span><span class="sxs-lookup"><span data-stu-id="8debc-129">id</span></span>             | <span data-ttu-id="8debc-130">String</span><span class="sxs-lookup"><span data-stu-id="8debc-130">String</span></span>  | <span data-ttu-id="8debc-131">Уникальный идентификатор конечной точки; Ключ.</span><span class="sxs-lookup"><span data-stu-id="8debc-131">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="8debc-132">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="8debc-132">Not nullable.</span></span> <span data-ttu-id="8debc-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8debc-133">Read-only.</span></span>|
| <span data-ttu-id="8debc-134">providerId</span><span class="sxs-lookup"><span data-stu-id="8debc-134">providerId</span></span>     | <span data-ttu-id="8debc-135">String</span><span class="sxs-lookup"><span data-stu-id="8debc-135">String</span></span>  | <span data-ttu-id="8debc-136">ИД приложения для службы публикации.</span><span class="sxs-lookup"><span data-stu-id="8debc-136">Application id of the publishing underlying service.</span></span> <span data-ttu-id="8debc-137">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="8debc-137">Not nullable.</span></span> <span data-ttu-id="8debc-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8debc-138">Read-only.</span></span>|
| <span data-ttu-id="8debc-139">providerName</span><span class="sxs-lookup"><span data-stu-id="8debc-139">providerName</span></span>   | <span data-ttu-id="8debc-140">String</span><span class="sxs-lookup"><span data-stu-id="8debc-140">String</span></span>  | <span data-ttu-id="8debc-141">Имя службы публикации.</span><span class="sxs-lookup"><span data-stu-id="8debc-141">Name of the publishing underlying service.</span></span> <span data-ttu-id="8debc-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8debc-142">Read-only.</span></span>|
| <span data-ttu-id="8debc-143">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="8debc-143">providerResourceId</span></span>|<span data-ttu-id="8debc-144">String</span><span class="sxs-lookup"><span data-stu-id="8debc-144">String</span></span>| <span data-ttu-id="8debc-145">Для групп Microsoft 365 это известное имя ресурса (например, Yammer.FeedURL и т. д.).</span><span class="sxs-lookup"><span data-stu-id="8debc-145">For Microsoft 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="8debc-146">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="8debc-146">Not nullable.</span></span> <span data-ttu-id="8debc-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8debc-147">Read-only.</span></span>|
| <span data-ttu-id="8debc-148">uri</span><span class="sxs-lookup"><span data-stu-id="8debc-148">uri</span></span>            | <span data-ttu-id="8debc-149">String</span><span class="sxs-lookup"><span data-stu-id="8debc-149">String</span></span>  | <span data-ttu-id="8debc-150">URL-адрес опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="8debc-150">URL of the published resource.</span></span> <span data-ttu-id="8debc-151">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="8debc-151">Not nullable.</span></span> <span data-ttu-id="8debc-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8debc-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8debc-153">Связи</span><span class="sxs-lookup"><span data-stu-id="8debc-153">Relationships</span></span>

<span data-ttu-id="8debc-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8debc-154">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8debc-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8debc-155">JSON representation</span></span>
<span data-ttu-id="8debc-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8debc-156">Here is a JSON representation of the resource.</span></span>

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


