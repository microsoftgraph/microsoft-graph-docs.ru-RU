---
title: Тип ресурса конечной точки
description: 'Конечные точки представляют собой URL-адреса для ресурсов, связанного с объектом.  Например при создании новой группы Office 365, дополнительные ресурсы также создаются как часть группы Office 365. К ним относятся почтового ящика группы для бесед и папка OneDrive группы для документов и файлов. Дополнительные сведения об этих ресурсах группы Office 365, включая их URL-адреса связанных ресурсов могут теперь читать с помощью панели навигации *конечных точек* на тип ресурсов группы. Это позволяет приложениям для понимания этих ресурсов и даже внедрение ресурсов, URL-адрес среды взаимодействия с пользователем в свои собственные каждый раз. '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512061"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="94d18-107">Тип ресурса конечной точки</span><span class="sxs-lookup"><span data-stu-id="94d18-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d18-108">Конечные точки представляют собой URL-адреса для ресурсов, связанного с объектом.</span><span class="sxs-lookup"><span data-stu-id="94d18-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="94d18-109">Например при создании новой группы Office 365, дополнительные ресурсы также создаются как часть группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="94d18-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="94d18-110">К ним относятся почтового ящика группы для бесед и папка OneDrive группы для документов и файлов.</span><span class="sxs-lookup"><span data-stu-id="94d18-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="94d18-111">Дополнительные сведения об этих ресурсах группы Office 365, включая их URL-адреса связанных ресурсов могут теперь читать с помощью панели навигации *конечных точек* на тип ресурсов группы.</span><span class="sxs-lookup"><span data-stu-id="94d18-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="94d18-112">Это позволяет приложениям для понимания этих ресурсов и даже внедрение ресурсов, URL-адрес среды взаимодействия с пользователем в свои собственные каждый раз.</span><span class="sxs-lookup"><span data-stu-id="94d18-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="94d18-113">Методы</span><span class="sxs-lookup"><span data-stu-id="94d18-113">Methods</span></span>

| <span data-ttu-id="94d18-114">Метод</span><span class="sxs-lookup"><span data-stu-id="94d18-114">Method</span></span>           | <span data-ttu-id="94d18-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="94d18-115">Return Type</span></span>    |<span data-ttu-id="94d18-116">Описание</span><span class="sxs-lookup"><span data-stu-id="94d18-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94d18-117">Перечисление конечных точек</span><span class="sxs-lookup"><span data-stu-id="94d18-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="94d18-118">Коллекция [Endpoint](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="94d18-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="94d18-119">Получение коллекции объектов endpoint.</span><span class="sxs-lookup"><span data-stu-id="94d18-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="94d18-120">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="94d18-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="94d18-121">Конечная точка</span><span class="sxs-lookup"><span data-stu-id="94d18-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="94d18-122">Чтение свойств и связей объекта endpoint.</span><span class="sxs-lookup"><span data-stu-id="94d18-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94d18-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="94d18-123">Properties</span></span>
| <span data-ttu-id="94d18-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="94d18-124">Property</span></span>     | <span data-ttu-id="94d18-125">Тип</span><span class="sxs-lookup"><span data-stu-id="94d18-125">Type</span></span>   |<span data-ttu-id="94d18-126">Описание</span><span class="sxs-lookup"><span data-stu-id="94d18-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94d18-127">Возможность</span><span class="sxs-lookup"><span data-stu-id="94d18-127">capability</span></span>     | <span data-ttu-id="94d18-128">String</span><span class="sxs-lookup"><span data-stu-id="94d18-128">String</span></span>  | <span data-ttu-id="94d18-129">Описание возможностей, связанный с этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="94d18-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="94d18-130">(например сообщения, беседы, и т.д.)  Не допускает значение NULL.</span><span class="sxs-lookup"><span data-stu-id="94d18-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="94d18-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94d18-131">Read-only.</span></span> |
| <span data-ttu-id="94d18-132">id</span><span class="sxs-lookup"><span data-stu-id="94d18-132">id</span></span>             | <span data-ttu-id="94d18-133">String</span><span class="sxs-lookup"><span data-stu-id="94d18-133">String</span></span>  | <span data-ttu-id="94d18-134">Уникальный идентификатор конечной точки; Ключ.</span><span class="sxs-lookup"><span data-stu-id="94d18-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="94d18-135">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="94d18-135">Not nullable.</span></span> <span data-ttu-id="94d18-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94d18-136">Read-only.</span></span>|
| <span data-ttu-id="94d18-137">ProviderID</span><span class="sxs-lookup"><span data-stu-id="94d18-137">providerId</span></span>     | <span data-ttu-id="94d18-138">String</span><span class="sxs-lookup"><span data-stu-id="94d18-138">String</span></span>  | <span data-ttu-id="94d18-139">Идентификатор приложения базовая служба публикации.</span><span class="sxs-lookup"><span data-stu-id="94d18-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="94d18-140">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="94d18-140">Not nullable.</span></span> <span data-ttu-id="94d18-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94d18-141">Read-only.</span></span>|
| <span data-ttu-id="94d18-142">ProviderName</span><span class="sxs-lookup"><span data-stu-id="94d18-142">providerName</span></span>   | <span data-ttu-id="94d18-143">String</span><span class="sxs-lookup"><span data-stu-id="94d18-143">String</span></span>  | <span data-ttu-id="94d18-144">Имя основного службы публикации.</span><span class="sxs-lookup"><span data-stu-id="94d18-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="94d18-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94d18-145">Read-only.</span></span>|
| <span data-ttu-id="94d18-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="94d18-146">providerResourceId</span></span>|<span data-ttu-id="94d18-147">String</span><span class="sxs-lookup"><span data-stu-id="94d18-147">String</span></span>| <span data-ttu-id="94d18-148">Для группы Office 365 устанавливается для хорошо известных имя ресурса (например Yammer.FeedURL и т.д.).</span><span class="sxs-lookup"><span data-stu-id="94d18-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="94d18-149">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="94d18-149">Not nullable.</span></span> <span data-ttu-id="94d18-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94d18-150">Read-only.</span></span>|
| <span data-ttu-id="94d18-151">URI</span><span class="sxs-lookup"><span data-stu-id="94d18-151">uri</span></span>            | <span data-ttu-id="94d18-152">String</span><span class="sxs-lookup"><span data-stu-id="94d18-152">String</span></span>  | <span data-ttu-id="94d18-153">URL-адрес опубликованных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="94d18-153">URL of the published resource.</span></span> <span data-ttu-id="94d18-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="94d18-154">Not nullable.</span></span> <span data-ttu-id="94d18-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94d18-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94d18-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="94d18-156">Relationships</span></span>

<span data-ttu-id="94d18-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="94d18-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="94d18-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="94d18-158">JSON representation</span></span>
<span data-ttu-id="94d18-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94d18-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
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
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
