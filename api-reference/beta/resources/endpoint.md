---
title: Тип ресурса конечной точки
description: 'Конечные точки представляют собой URL-адреса для ресурсов, связанного с объектом.  Например при создании новой группы Office 365, дополнительные ресурсы также создаются как часть группы Office 365. К ним относятся почтового ящика группы для бесед и папка OneDrive группы для документов и файлов. Дополнительные сведения об этих ресурсах группы Office 365, включая их URL-адреса связанных ресурсов могут теперь читать с помощью панели навигации *конечных точек* на тип ресурсов группы. Это позволяет приложениям для понимания этих ресурсов и даже внедрение ресурсов, URL-адрес среды взаимодействия с пользователем в свои собственные каждый раз. '
ms.openlocfilehash: 8d95cef8e25095512e94d5aed5ec7540562862bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076444"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="79b6e-107">Тип ресурса конечной точки</span><span class="sxs-lookup"><span data-stu-id="79b6e-107">Endpoint resource type</span></span>

> <span data-ttu-id="79b6e-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="79b6e-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79b6e-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79b6e-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79b6e-110">Конечные точки представляют собой URL-адреса для ресурсов, связанного с объектом.</span><span class="sxs-lookup"><span data-stu-id="79b6e-110">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="79b6e-111">Например при создании новой группы Office 365, дополнительные ресурсы также создаются как часть группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="79b6e-111">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="79b6e-112">К ним относятся почтового ящика группы для бесед и папка OneDrive группы для документов и файлов.</span><span class="sxs-lookup"><span data-stu-id="79b6e-112">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="79b6e-113">Дополнительные сведения об этих ресурсах группы Office 365, включая их URL-адреса связанных ресурсов могут теперь читать с помощью панели навигации *конечных точек* на тип ресурсов группы.</span><span class="sxs-lookup"><span data-stu-id="79b6e-113">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="79b6e-114">Это позволяет приложениям для понимания этих ресурсов и даже внедрение ресурсов, URL-адрес среды взаимодействия с пользователем в свои собственные каждый раз.</span><span class="sxs-lookup"><span data-stu-id="79b6e-114">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="79b6e-115">Методы</span><span class="sxs-lookup"><span data-stu-id="79b6e-115">Methods</span></span>

| <span data-ttu-id="79b6e-116">Метод</span><span class="sxs-lookup"><span data-stu-id="79b6e-116">Method</span></span>           | <span data-ttu-id="79b6e-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="79b6e-117">Return Type</span></span>    |<span data-ttu-id="79b6e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="79b6e-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79b6e-119">Список конечных точек</span><span class="sxs-lookup"><span data-stu-id="79b6e-119">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="79b6e-120">Коллекция [конечных точек](endpoint.md)</span><span class="sxs-lookup"><span data-stu-id="79b6e-120">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="79b6e-121">Получение коллекции объектов конечной точки.</span><span class="sxs-lookup"><span data-stu-id="79b6e-121">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="79b6e-122">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="79b6e-122">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="79b6e-123">Конечная точка</span><span class="sxs-lookup"><span data-stu-id="79b6e-123">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="79b6e-124">Чтение свойства и связи объекта конечной точки.</span><span class="sxs-lookup"><span data-stu-id="79b6e-124">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="79b6e-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="79b6e-125">Properties</span></span>
| <span data-ttu-id="79b6e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="79b6e-126">Property</span></span>     | <span data-ttu-id="79b6e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="79b6e-127">Type</span></span>   |<span data-ttu-id="79b6e-128">Description</span><span class="sxs-lookup"><span data-stu-id="79b6e-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79b6e-129">возможность</span><span class="sxs-lookup"><span data-stu-id="79b6e-129">capability</span></span>     | <span data-ttu-id="79b6e-130">String</span><span class="sxs-lookup"><span data-stu-id="79b6e-130">String</span></span>  | <span data-ttu-id="79b6e-131">Описание возможностей, связанный с этим ресурсом.</span><span class="sxs-lookup"><span data-stu-id="79b6e-131">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="79b6e-132">(например сообщения, беседы, и т.д.)  Не допускает значение NULL.</span><span class="sxs-lookup"><span data-stu-id="79b6e-132">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="79b6e-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79b6e-133">Read-only.</span></span> |
| <span data-ttu-id="79b6e-134">id</span><span class="sxs-lookup"><span data-stu-id="79b6e-134">id</span></span>             | <span data-ttu-id="79b6e-135">String</span><span class="sxs-lookup"><span data-stu-id="79b6e-135">String</span></span>  | <span data-ttu-id="79b6e-136">Уникальный идентификатор конечной точки; Ключ.</span><span class="sxs-lookup"><span data-stu-id="79b6e-136">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="79b6e-137">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="79b6e-137">Not nullable.</span></span> <span data-ttu-id="79b6e-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79b6e-138">Read-only.</span></span>|
| <span data-ttu-id="79b6e-139">providerId</span><span class="sxs-lookup"><span data-stu-id="79b6e-139">providerId</span></span>     | <span data-ttu-id="79b6e-140">String</span><span class="sxs-lookup"><span data-stu-id="79b6e-140">String</span></span>  | <span data-ttu-id="79b6e-141">Идентификатор приложения базовая служба публикации.</span><span class="sxs-lookup"><span data-stu-id="79b6e-141">Application id of the publishing underlying service.</span></span> <span data-ttu-id="79b6e-142">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="79b6e-142">Not nullable.</span></span> <span data-ttu-id="79b6e-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79b6e-143">Read-only.</span></span>|
| <span data-ttu-id="79b6e-144">providerName</span><span class="sxs-lookup"><span data-stu-id="79b6e-144">providerName</span></span>   | <span data-ttu-id="79b6e-145">String</span><span class="sxs-lookup"><span data-stu-id="79b6e-145">String</span></span>  | <span data-ttu-id="79b6e-146">Имя основного службы публикации.</span><span class="sxs-lookup"><span data-stu-id="79b6e-146">Name of the publishing underlying service.</span></span> <span data-ttu-id="79b6e-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79b6e-147">Read-only.</span></span>|
| <span data-ttu-id="79b6e-148">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="79b6e-148">providerResourceId</span></span>|<span data-ttu-id="79b6e-149">String</span><span class="sxs-lookup"><span data-stu-id="79b6e-149">String</span></span>| <span data-ttu-id="79b6e-150">Для группы Office 365 устанавливается для хорошо известных имя ресурса (например Yammer.FeedURL и т.д.).</span><span class="sxs-lookup"><span data-stu-id="79b6e-150">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="79b6e-151">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="79b6e-151">Not nullable.</span></span> <span data-ttu-id="79b6e-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79b6e-152">Read-only.</span></span>|
| <span data-ttu-id="79b6e-153">URI</span><span class="sxs-lookup"><span data-stu-id="79b6e-153">uri</span></span>            | <span data-ttu-id="79b6e-154">String</span><span class="sxs-lookup"><span data-stu-id="79b6e-154">String</span></span>  | <span data-ttu-id="79b6e-155">URL-адрес опубликованных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="79b6e-155">URL of the published resource.</span></span> <span data-ttu-id="79b6e-156">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="79b6e-156">Not nullable.</span></span> <span data-ttu-id="79b6e-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="79b6e-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79b6e-158">Связи</span><span class="sxs-lookup"><span data-stu-id="79b6e-158">Relationships</span></span>

<span data-ttu-id="79b6e-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="79b6e-159">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="79b6e-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="79b6e-160">JSON representation</span></span>
<span data-ttu-id="79b6e-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79b6e-161">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->