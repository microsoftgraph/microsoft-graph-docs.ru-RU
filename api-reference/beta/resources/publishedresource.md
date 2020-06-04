---
title: Тип ресурса Публишедресаурце
description: Тип ресурса Публишедресаурце.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d42464fa6e249fef8d7b535b6327751f48d17167
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556326"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="61b2d-103">Тип ресурса Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="61b2d-103">publishedResource resource type</span></span>

<span data-ttu-id="61b2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61b2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61b2d-105">Представляет локальный опубликованный ресурс.</span><span class="sxs-lookup"><span data-stu-id="61b2d-105">Represents on-premises published resource.</span></span> <span data-ttu-id="61b2d-106">Администратор клиента может публиковать различные типы локальных ресурсов, корпоративных приложений, контроллеров домена, серверов и т. д. [локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному опубликованному ресурсу или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="61b2d-106">A tenant administrator can publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="61b2d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="61b2d-107">Methods</span></span>

| <span data-ttu-id="61b2d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="61b2d-108">Method</span></span>       | <span data-ttu-id="61b2d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61b2d-109">Return Type</span></span> | <span data-ttu-id="61b2d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="61b2d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="61b2d-111">Список Публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="61b2d-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="61b2d-112">Коллекция объектов [публишедресаурце](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="61b2d-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="61b2d-113">Получение коллекции объектов **публишедресаурцес** .</span><span class="sxs-lookup"><span data-stu-id="61b2d-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="61b2d-114">Получение Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="61b2d-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="61b2d-115">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="61b2d-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="61b2d-116">Чтение свойств и связей объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="61b2d-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="61b2d-117">Создание Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="61b2d-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="61b2d-118">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="61b2d-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="61b2d-119">Создание нового **публишедресаурце**.</span><span class="sxs-lookup"><span data-stu-id="61b2d-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="61b2d-120">Обновление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="61b2d-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="61b2d-121">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="61b2d-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="61b2d-122">Обновление объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="61b2d-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="61b2d-123">Удаление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="61b2d-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="61b2d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="61b2d-124">None</span></span> | <span data-ttu-id="61b2d-125">Удаление объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="61b2d-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="61b2d-126">Назначение Публишедресаурце для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="61b2d-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="61b2d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="61b2d-127">None</span></span> | <span data-ttu-id="61b2d-128">Назначьте объект **публишедресаурце** для **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="61b2d-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="61b2d-129">Удаление Публишедресаурце из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="61b2d-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="61b2d-130">Нет</span><span class="sxs-lookup"><span data-stu-id="61b2d-130">None</span></span> |  <span data-ttu-id="61b2d-131">Удаление объекта **публишедресаурце** из объекта **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="61b2d-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="61b2d-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="61b2d-132">Properties</span></span>

| <span data-ttu-id="61b2d-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="61b2d-133">Property</span></span>     | <span data-ttu-id="61b2d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="61b2d-134">Type</span></span>        | <span data-ttu-id="61b2d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="61b2d-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61b2d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="61b2d-136">displayName</span></span>|<span data-ttu-id="61b2d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="61b2d-137">String</span></span>| <span data-ttu-id="61b2d-138">Отображаемое имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="61b2d-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="61b2d-139">id</span><span class="sxs-lookup"><span data-stu-id="61b2d-139">id</span></span>|<span data-ttu-id="61b2d-140">String</span><span class="sxs-lookup"><span data-stu-id="61b2d-140">String</span></span>| <span data-ttu-id="61b2d-141">Идентификатор объекта Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="61b2d-141">The object id of the publishedResource.</span></span> <span data-ttu-id="61b2d-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61b2d-142">Read-only.</span></span>|
|<span data-ttu-id="61b2d-143">публишингтипе</span><span class="sxs-lookup"><span data-stu-id="61b2d-143">publishingType</span></span>|<span data-ttu-id="61b2d-144">string</span><span class="sxs-lookup"><span data-stu-id="61b2d-144">string</span></span>| <span data-ttu-id="61b2d-145">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="61b2d-145">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="61b2d-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="61b2d-146">resourceName</span></span>|<span data-ttu-id="61b2d-147">String</span><span class="sxs-lookup"><span data-stu-id="61b2d-147">String</span></span>|<span data-ttu-id="61b2d-148">Имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="61b2d-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61b2d-149">Связи</span><span class="sxs-lookup"><span data-stu-id="61b2d-149">Relationships</span></span>

| <span data-ttu-id="61b2d-150">Связь</span><span class="sxs-lookup"><span data-stu-id="61b2d-150">Relationship</span></span> | <span data-ttu-id="61b2d-151">Тип</span><span class="sxs-lookup"><span data-stu-id="61b2d-151">Type</span></span>        | <span data-ttu-id="61b2d-152">Описание</span><span class="sxs-lookup"><span data-stu-id="61b2d-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61b2d-153">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="61b2d-153">agentGroups</span></span>|<span data-ttu-id="61b2d-154">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="61b2d-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="61b2d-155">Список **онпремисесажентграупс** , которым назначено **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="61b2d-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="61b2d-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61b2d-156">Read-only.</span></span> <span data-ttu-id="61b2d-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="61b2d-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61b2d-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61b2d-158">JSON representation</span></span>

<span data-ttu-id="61b2d-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61b2d-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publishedResource",
  "baseType": "",
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
