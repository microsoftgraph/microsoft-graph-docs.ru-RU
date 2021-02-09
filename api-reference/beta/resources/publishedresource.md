---
title: Тип ресурса publishedResource
description: Тип ресурса publishedResource.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1090e985fc9ffdec0c27f9793a361851d2fa5216
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155568"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="4be3a-103">Тип ресурса publishedResource</span><span class="sxs-lookup"><span data-stu-id="4be3a-103">publishedResource resource type</span></span>

<span data-ttu-id="4be3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4be3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be3a-105">Представляет локально опубликованный ресурс.</span><span class="sxs-lookup"><span data-stu-id="4be3a-105">Represents on-premises published resource.</span></span> <span data-ttu-id="4be3a-106">Администратор клиента может публиковать различные типы локального ресурса — корпоративные приложения, контроллеры домена, серверы и [т.](onpremisesagent.md) д. Установленные администратором клиента локально агенты можно настроить для доступа к определенному опубликованного ресурса и обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="4be3a-106">A tenant administrator can publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="4be3a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4be3a-107">Methods</span></span>

| <span data-ttu-id="4be3a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4be3a-108">Method</span></span>       | <span data-ttu-id="4be3a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4be3a-109">Return Type</span></span> | <span data-ttu-id="4be3a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4be3a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4be3a-111">Список publishedResources</span><span class="sxs-lookup"><span data-stu-id="4be3a-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="4be3a-112">[Коллекция объектов publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="4be3a-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="4be3a-113">Получите **коллекцию объектов publishedResources.**</span><span class="sxs-lookup"><span data-stu-id="4be3a-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="4be3a-114">Get publishedResource</span><span class="sxs-lookup"><span data-stu-id="4be3a-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="4be3a-115">publishedResource</span><span class="sxs-lookup"><span data-stu-id="4be3a-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="4be3a-116">Чтение свойств и связей объекта **publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="4be3a-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="4be3a-117">Создание publishedResource</span><span class="sxs-lookup"><span data-stu-id="4be3a-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="4be3a-118">publishedResource</span><span class="sxs-lookup"><span data-stu-id="4be3a-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="4be3a-119">Создание нового **publishedResource**.</span><span class="sxs-lookup"><span data-stu-id="4be3a-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="4be3a-120">Обновление publishedResource</span><span class="sxs-lookup"><span data-stu-id="4be3a-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="4be3a-121">publishedResource</span><span class="sxs-lookup"><span data-stu-id="4be3a-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="4be3a-122">Обновление объекта **publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="4be3a-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="4be3a-123">Удаление publishedResource</span><span class="sxs-lookup"><span data-stu-id="4be3a-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="4be3a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4be3a-124">None</span></span> | <span data-ttu-id="4be3a-125">Удаление объекта **publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="4be3a-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="4be3a-126">Назначение publishedResource onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="4be3a-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="4be3a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="4be3a-127">None</span></span> | <span data-ttu-id="4be3a-128">**Назначьте объект publishedResource** **объекту onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="4be3a-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="4be3a-129">Удаление publishedResource из onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="4be3a-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="4be3a-130">Нет</span><span class="sxs-lookup"><span data-stu-id="4be3a-130">None</span></span> |  <span data-ttu-id="4be3a-131">Удаление объекта **publishedResource** из **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="4be3a-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="4be3a-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="4be3a-132">Properties</span></span>

| <span data-ttu-id="4be3a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="4be3a-133">Property</span></span>     | <span data-ttu-id="4be3a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="4be3a-134">Type</span></span>        | <span data-ttu-id="4be3a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="4be3a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4be3a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4be3a-136">displayName</span></span>|<span data-ttu-id="4be3a-137">String</span><span class="sxs-lookup"><span data-stu-id="4be3a-137">String</span></span>| <span data-ttu-id="4be3a-138">Отображаемого имени publishedResource.</span><span class="sxs-lookup"><span data-stu-id="4be3a-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="4be3a-139">id</span><span class="sxs-lookup"><span data-stu-id="4be3a-139">id</span></span>|<span data-ttu-id="4be3a-140">String</span><span class="sxs-lookup"><span data-stu-id="4be3a-140">String</span></span>| <span data-ttu-id="4be3a-141">ИД объекта publishedResource.</span><span class="sxs-lookup"><span data-stu-id="4be3a-141">The object id of the publishedResource.</span></span> <span data-ttu-id="4be3a-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4be3a-142">Read-only.</span></span>|
|<span data-ttu-id="4be3a-143">publishingType</span><span class="sxs-lookup"><span data-stu-id="4be3a-143">publishingType</span></span>|<span data-ttu-id="4be3a-144">string</span><span class="sxs-lookup"><span data-stu-id="4be3a-144">string</span></span>| <span data-ttu-id="4be3a-145">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="4be3a-145">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="4be3a-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="4be3a-146">resourceName</span></span>|<span data-ttu-id="4be3a-147">String</span><span class="sxs-lookup"><span data-stu-id="4be3a-147">String</span></span>|<span data-ttu-id="4be3a-148">Имя publishedResource.</span><span class="sxs-lookup"><span data-stu-id="4be3a-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4be3a-149">Связи</span><span class="sxs-lookup"><span data-stu-id="4be3a-149">Relationships</span></span>

| <span data-ttu-id="4be3a-150">Связь</span><span class="sxs-lookup"><span data-stu-id="4be3a-150">Relationship</span></span> | <span data-ttu-id="4be3a-151">Тип</span><span class="sxs-lookup"><span data-stu-id="4be3a-151">Type</span></span>        | <span data-ttu-id="4be3a-152">Описание</span><span class="sxs-lookup"><span data-stu-id="4be3a-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4be3a-153">agentGroups</span><span class="sxs-lookup"><span data-stu-id="4be3a-153">agentGroups</span></span>|<span data-ttu-id="4be3a-154">[Коллекция onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="4be3a-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="4be3a-155">Список **onPremisesAgentGroups,** которые **назначены publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="4be3a-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="4be3a-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4be3a-156">Read-only.</span></span> <span data-ttu-id="4be3a-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4be3a-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4be3a-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4be3a-158">JSON representation</span></span>

<span data-ttu-id="4be3a-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4be3a-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "publishingType": "string",
  "resourceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "publishedResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


