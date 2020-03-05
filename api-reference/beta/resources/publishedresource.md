---
title: Тип ресурса Публишедресаурце
description: Тип ресурса Публишедресаурце.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7b6f81f9e3a6b399f7e029e21330fe83b533af87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521294"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="af9d9-103">Тип ресурса Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="af9d9-103">publishedResource resource type</span></span>

<span data-ttu-id="af9d9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="af9d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af9d9-105">Представляет локальный опубликованный ресурс.</span><span class="sxs-lookup"><span data-stu-id="af9d9-105">Represents on-premises published resource.</span></span> <span data-ttu-id="af9d9-106">Администратор клиента может публиковать различные типы локальных ресурсов, корпоративных приложений, контроллеров домена, серверов и т. д. [локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному опубликованному ресурсу или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="af9d9-106">A tenant administrator could publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="af9d9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="af9d9-107">Methods</span></span>

| <span data-ttu-id="af9d9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="af9d9-108">Method</span></span>       | <span data-ttu-id="af9d9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="af9d9-109">Return Type</span></span> | <span data-ttu-id="af9d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af9d9-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="af9d9-111">Список Публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="af9d9-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="af9d9-112">Коллекция объектов [публишедресаурце](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="af9d9-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="af9d9-113">Получение коллекции объектов **публишедресаурцес** .</span><span class="sxs-lookup"><span data-stu-id="af9d9-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="af9d9-114">Получение Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="af9d9-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="af9d9-115">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="af9d9-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="af9d9-116">Чтение свойств и связей объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="af9d9-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="af9d9-117">Создание Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="af9d9-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="af9d9-118">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="af9d9-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="af9d9-119">Создание нового **публишедресаурце**.</span><span class="sxs-lookup"><span data-stu-id="af9d9-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="af9d9-120">Обновление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="af9d9-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="af9d9-121">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="af9d9-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="af9d9-122">Обновление объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="af9d9-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="af9d9-123">Удаление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="af9d9-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="af9d9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="af9d9-124">None</span></span> | <span data-ttu-id="af9d9-125">Удаление объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="af9d9-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="af9d9-126">Назначение Публишедресаурце для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="af9d9-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="af9d9-127">Нет</span><span class="sxs-lookup"><span data-stu-id="af9d9-127">None</span></span> | <span data-ttu-id="af9d9-128">Назначьте объект **публишедресаурце** для **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="af9d9-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="af9d9-129">Удаление Публишедресаурце из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="af9d9-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="af9d9-130">Нет</span><span class="sxs-lookup"><span data-stu-id="af9d9-130">None</span></span> |  <span data-ttu-id="af9d9-131">Удаление объекта **публишедресаурце** из объекта **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="af9d9-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="af9d9-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="af9d9-132">Properties</span></span>

| <span data-ttu-id="af9d9-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="af9d9-133">Property</span></span>     | <span data-ttu-id="af9d9-134">Тип</span><span class="sxs-lookup"><span data-stu-id="af9d9-134">Type</span></span>        | <span data-ttu-id="af9d9-135">Описание</span><span class="sxs-lookup"><span data-stu-id="af9d9-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af9d9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="af9d9-136">displayName</span></span>|<span data-ttu-id="af9d9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="af9d9-137">String</span></span>| <span data-ttu-id="af9d9-138">Отображаемое имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="af9d9-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="af9d9-139">id</span><span class="sxs-lookup"><span data-stu-id="af9d9-139">id</span></span>|<span data-ttu-id="af9d9-140">String</span><span class="sxs-lookup"><span data-stu-id="af9d9-140">String</span></span>| <span data-ttu-id="af9d9-141">Идентификатор объекта Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="af9d9-141">The object id of the publishedResource.</span></span> <span data-ttu-id="af9d9-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af9d9-142">Read-only.</span></span>|
|<span data-ttu-id="af9d9-143">публишингтипе</span><span class="sxs-lookup"><span data-stu-id="af9d9-143">publishingType</span></span>|<span data-ttu-id="af9d9-144">строка</span><span class="sxs-lookup"><span data-stu-id="af9d9-144">string</span></span>| <span data-ttu-id="af9d9-145">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="af9d9-145">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="af9d9-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="af9d9-146">resourceName</span></span>|<span data-ttu-id="af9d9-147">String</span><span class="sxs-lookup"><span data-stu-id="af9d9-147">String</span></span>|<span data-ttu-id="af9d9-148">Имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="af9d9-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af9d9-149">Связи</span><span class="sxs-lookup"><span data-stu-id="af9d9-149">Relationships</span></span>

| <span data-ttu-id="af9d9-150">Связь</span><span class="sxs-lookup"><span data-stu-id="af9d9-150">Relationship</span></span> | <span data-ttu-id="af9d9-151">Тип</span><span class="sxs-lookup"><span data-stu-id="af9d9-151">Type</span></span>        | <span data-ttu-id="af9d9-152">Описание</span><span class="sxs-lookup"><span data-stu-id="af9d9-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="af9d9-153">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="af9d9-153">agentGroups</span></span>|<span data-ttu-id="af9d9-154">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="af9d9-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="af9d9-155">Список **онпремисесажентграупс** , которым назначено **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="af9d9-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="af9d9-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af9d9-156">Read-only.</span></span> <span data-ttu-id="af9d9-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="af9d9-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af9d9-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af9d9-158">JSON representation</span></span>

<span data-ttu-id="af9d9-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af9d9-159">The following is a JSON representation of the resource.</span></span>

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
