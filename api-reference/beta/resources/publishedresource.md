---
title: Тип ресурса Публишедресаурце
description: Тип ресурса Публишедресаурце.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54a2b1b610f30ec3ce7d9853916aad345142cbf0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841362"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="da41e-103">Тип ресурса Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="da41e-103">publishedResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da41e-104">Представляет локальный опубликованный ресурс.</span><span class="sxs-lookup"><span data-stu-id="da41e-104">Represents on-premises published resource.</span></span> <span data-ttu-id="da41e-105">Администратор клиента может публиковать различные типы локальных ресурсов, корпоративных приложений, контроллеров домена, серверов и т. д. [локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к ним и обработки запросов к определенный опубликованный ресурс.</span><span class="sxs-lookup"><span data-stu-id="da41e-105">A tenant administrator could publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="da41e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="da41e-106">Methods</span></span>

| <span data-ttu-id="da41e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="da41e-107">Method</span></span>       | <span data-ttu-id="da41e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da41e-108">Return Type</span></span> | <span data-ttu-id="da41e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="da41e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="da41e-110">Список Публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="da41e-110">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="da41e-111">Коллекция объектов [публишедресаурце](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="da41e-111">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="da41e-112">Получение коллекции объектов **публишедресаурцес** .</span><span class="sxs-lookup"><span data-stu-id="da41e-112">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="da41e-113">Получение Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="da41e-113">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="da41e-114">Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="da41e-114">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="da41e-115">Чтение свойств и связей объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="da41e-115">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="da41e-116">Создание Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="da41e-116">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="da41e-117">Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="da41e-117">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="da41e-118">Создание нового **публишедресаурце**.</span><span class="sxs-lookup"><span data-stu-id="da41e-118">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="da41e-119">Обновление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="da41e-119">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="da41e-120">Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="da41e-120">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="da41e-121">Обновление объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="da41e-121">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="da41e-122">Удаление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="da41e-122">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="da41e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="da41e-123">None</span></span> | <span data-ttu-id="da41e-124">Удаление объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="da41e-124">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="da41e-125">Назначение Публишедресаурце для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="da41e-125">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="da41e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="da41e-126">None</span></span> | <span data-ttu-id="da41e-127">Назначьте объект **публишедресаурце** для **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="da41e-127">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="da41e-128">Удаление Публишедресаурце из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="da41e-128">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="da41e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="da41e-129">None</span></span> |  <span data-ttu-id="da41e-130">Удаление объекта **публишедресаурце** из объекта **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="da41e-130">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="da41e-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="da41e-131">Properties</span></span>

| <span data-ttu-id="da41e-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="da41e-132">Property</span></span>     | <span data-ttu-id="da41e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="da41e-133">Type</span></span>        | <span data-ttu-id="da41e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="da41e-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da41e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="da41e-135">displayName</span></span>|<span data-ttu-id="da41e-136">Строка</span><span class="sxs-lookup"><span data-stu-id="da41e-136">String</span></span>| <span data-ttu-id="da41e-137">Отображаемое имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="da41e-137">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="da41e-138">id</span><span class="sxs-lookup"><span data-stu-id="da41e-138">id</span></span>|<span data-ttu-id="da41e-139">String</span><span class="sxs-lookup"><span data-stu-id="da41e-139">String</span></span>| <span data-ttu-id="da41e-140">Идентификатор объекта Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="da41e-140">The object id of the publishedResource.</span></span> <span data-ttu-id="da41e-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da41e-141">Read-only.</span></span>|
|<span data-ttu-id="da41e-142">Публишингтипе</span><span class="sxs-lookup"><span data-stu-id="da41e-142">publishingType</span></span>|<span data-ttu-id="da41e-143">string</span><span class="sxs-lookup"><span data-stu-id="da41e-143">string</span></span>| <span data-ttu-id="da41e-144">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="da41e-144">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="da41e-145">resourceName</span><span class="sxs-lookup"><span data-stu-id="da41e-145">resourceName</span></span>|<span data-ttu-id="da41e-146">String</span><span class="sxs-lookup"><span data-stu-id="da41e-146">String</span></span>|<span data-ttu-id="da41e-147">Имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="da41e-147">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da41e-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="da41e-148">Relationships</span></span>

| <span data-ttu-id="da41e-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="da41e-149">Relationship</span></span> | <span data-ttu-id="da41e-150">Тип</span><span class="sxs-lookup"><span data-stu-id="da41e-150">Type</span></span>        | <span data-ttu-id="da41e-151">Описание</span><span class="sxs-lookup"><span data-stu-id="da41e-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da41e-152">Ажентграупс</span><span class="sxs-lookup"><span data-stu-id="da41e-152">agentGroups</span></span>|<span data-ttu-id="da41e-153">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="da41e-153">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="da41e-154">Список **онпремисесажентграупс** , которым назначено **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="da41e-154">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="da41e-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da41e-155">Read-only.</span></span> <span data-ttu-id="da41e-156">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="da41e-156">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da41e-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da41e-157">JSON representation</span></span>

<span data-ttu-id="da41e-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da41e-158">The following is a JSON representation of the resource.</span></span>

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
