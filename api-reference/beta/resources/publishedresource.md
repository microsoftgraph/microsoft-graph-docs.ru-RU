---
title: тип ресурса publishedResource
description: тип ресурса publishedResource.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: eb28f345aba008a0f2d5bb5ab4723c2ffbb8aca3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760934"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="eda3c-103">тип ресурса publishedResource</span><span class="sxs-lookup"><span data-stu-id="eda3c-103">publishedResource resource type</span></span>

<span data-ttu-id="eda3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eda3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eda3c-105">Представляет локально опубликованный ресурс.</span><span class="sxs-lookup"><span data-stu-id="eda3c-105">Represents on-premises published resource.</span></span> <span data-ttu-id="eda3c-106">Администратор клиента может публиковать различные типы локального ресурса — корпоративные приложения, контроллеры доменов, серверы и [т.](onpremisesagent.md) д. Агенты, установленные администратором клиента, могут быть настроены для доступа и обработки запросов к конкретному опубликованому ресурсу.</span><span class="sxs-lookup"><span data-stu-id="eda3c-106">A tenant administrator can publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="eda3c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="eda3c-107">Methods</span></span>

| <span data-ttu-id="eda3c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="eda3c-108">Method</span></span>       | <span data-ttu-id="eda3c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eda3c-109">Return Type</span></span> | <span data-ttu-id="eda3c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eda3c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eda3c-111">Список опубликованныхResources</span><span class="sxs-lookup"><span data-stu-id="eda3c-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="eda3c-112">[коллекция объектов publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="eda3c-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="eda3c-113">Получите **коллекцию объектов publishedResources.**</span><span class="sxs-lookup"><span data-stu-id="eda3c-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="eda3c-114">Get publishedResource</span><span class="sxs-lookup"><span data-stu-id="eda3c-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="eda3c-115">publishedResource</span><span class="sxs-lookup"><span data-stu-id="eda3c-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="eda3c-116">Ознакомьтесь с свойствами и отношениями объекта **publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="eda3c-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="eda3c-117">Создание publishedResource</span><span class="sxs-lookup"><span data-stu-id="eda3c-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="eda3c-118">publishedResource</span><span class="sxs-lookup"><span data-stu-id="eda3c-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="eda3c-119">Создание нового **publishedResource**.</span><span class="sxs-lookup"><span data-stu-id="eda3c-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="eda3c-120">Update publishedResource</span><span class="sxs-lookup"><span data-stu-id="eda3c-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="eda3c-121">publishedResource</span><span class="sxs-lookup"><span data-stu-id="eda3c-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="eda3c-122">Обновление **объекта publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="eda3c-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="eda3c-123">Удаление publishedResource</span><span class="sxs-lookup"><span data-stu-id="eda3c-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="eda3c-124">Нет</span><span class="sxs-lookup"><span data-stu-id="eda3c-124">None</span></span> | <span data-ttu-id="eda3c-125">Удаление **объекта publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="eda3c-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="eda3c-126">Назначение publishedResource onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="eda3c-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="eda3c-127">Нет</span><span class="sxs-lookup"><span data-stu-id="eda3c-127">None</span></span> | <span data-ttu-id="eda3c-128">Назначение **объекта publishedResource** в **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="eda3c-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="eda3c-129">Удаление publishedResource из onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="eda3c-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="eda3c-130">Нет</span><span class="sxs-lookup"><span data-stu-id="eda3c-130">None</span></span> |  <span data-ttu-id="eda3c-131">Удалите **объект publishedResource** из **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="eda3c-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="eda3c-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="eda3c-132">Properties</span></span>

| <span data-ttu-id="eda3c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="eda3c-133">Property</span></span>     | <span data-ttu-id="eda3c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="eda3c-134">Type</span></span>        | <span data-ttu-id="eda3c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="eda3c-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eda3c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eda3c-136">displayName</span></span>|<span data-ttu-id="eda3c-137">String</span><span class="sxs-lookup"><span data-stu-id="eda3c-137">String</span></span>| <span data-ttu-id="eda3c-138">Отображение имени опубликованногоРесурса.</span><span class="sxs-lookup"><span data-stu-id="eda3c-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="eda3c-139">id</span><span class="sxs-lookup"><span data-stu-id="eda3c-139">id</span></span>|<span data-ttu-id="eda3c-140">String</span><span class="sxs-lookup"><span data-stu-id="eda3c-140">String</span></span>| <span data-ttu-id="eda3c-141">ID объекта publishedResource.</span><span class="sxs-lookup"><span data-stu-id="eda3c-141">The object id of the publishedResource.</span></span> <span data-ttu-id="eda3c-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eda3c-142">Read-only.</span></span>|
|<span data-ttu-id="eda3c-143">publishingType</span><span class="sxs-lookup"><span data-stu-id="eda3c-143">publishingType</span></span>|<span data-ttu-id="eda3c-144">string</span><span class="sxs-lookup"><span data-stu-id="eda3c-144">string</span></span>| <span data-ttu-id="eda3c-145">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="eda3c-145">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="eda3c-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="eda3c-146">resourceName</span></span>|<span data-ttu-id="eda3c-147">String</span><span class="sxs-lookup"><span data-stu-id="eda3c-147">String</span></span>|<span data-ttu-id="eda3c-148">Имя опубликованногоResource.</span><span class="sxs-lookup"><span data-stu-id="eda3c-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eda3c-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="eda3c-149">Relationships</span></span>

| <span data-ttu-id="eda3c-150">Связь</span><span class="sxs-lookup"><span data-stu-id="eda3c-150">Relationship</span></span> | <span data-ttu-id="eda3c-151">Тип</span><span class="sxs-lookup"><span data-stu-id="eda3c-151">Type</span></span>        | <span data-ttu-id="eda3c-152">Описание</span><span class="sxs-lookup"><span data-stu-id="eda3c-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eda3c-153">agentGroups</span><span class="sxs-lookup"><span data-stu-id="eda3c-153">agentGroups</span></span>|<span data-ttu-id="eda3c-154">[коллекция onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="eda3c-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="eda3c-155">Список **onPremisesAgentGroups,** которые **назначены публикацииResource.**</span><span class="sxs-lookup"><span data-stu-id="eda3c-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="eda3c-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eda3c-156">Read-only.</span></span> <span data-ttu-id="eda3c-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="eda3c-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eda3c-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eda3c-158">JSON representation</span></span>

<span data-ttu-id="eda3c-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eda3c-159">The following is a JSON representation of the resource.</span></span>

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


