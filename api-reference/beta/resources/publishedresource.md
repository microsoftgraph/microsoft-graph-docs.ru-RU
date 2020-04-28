---
title: Тип ресурса Публишедресаурце
description: Тип ресурса Публишедресаурце.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d57ede14ba5c5d392c0a2a0388e1757cc481242c
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199993"
---
# <a name="publishedresource-resource-type"></a><span data-ttu-id="0ffa5-103">Тип ресурса Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="0ffa5-103">publishedResource resource type</span></span>

<span data-ttu-id="0ffa5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ffa5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ffa5-105">Представляет локальный опубликованный ресурс.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-105">Represents on-premises published resource.</span></span> <span data-ttu-id="0ffa5-106">Администратор клиента может публиковать различные типы локальных ресурсов, корпоративных приложений, контроллеров домена, серверов и т. д. [локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному опубликованному ресурсу или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-106">A tenant administrator could publish various types of on-premises resources - enterprise applications, domain controllers, servers, etc. [On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular published resource.</span></span>

## <a name="methods"></a><span data-ttu-id="0ffa5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0ffa5-107">Methods</span></span>

| <span data-ttu-id="0ffa5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0ffa5-108">Method</span></span>       | <span data-ttu-id="0ffa5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0ffa5-109">Return Type</span></span> | <span data-ttu-id="0ffa5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0ffa5-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0ffa5-111">Список Публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="0ffa5-111">List publishedResources</span></span>](../api/publishedresource-list.md) | <span data-ttu-id="0ffa5-112">Коллекция объектов [публишедресаурце](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="0ffa5-112">[publishedResource](publishedresource.md) objects collection</span></span> | <span data-ttu-id="0ffa5-113">Получение коллекции объектов **публишедресаурцес** .</span><span class="sxs-lookup"><span data-stu-id="0ffa5-113">Get a **publishedResources** object collection.</span></span> |
| [<span data-ttu-id="0ffa5-114">Получение Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="0ffa5-114">Get publishedResource</span></span>](../api/publishedresource-get.md) | [<span data-ttu-id="0ffa5-115">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="0ffa5-115">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="0ffa5-116">Чтение свойств и связей объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="0ffa5-116">Read the properties and relationships of a **publishedResource** object.</span></span> |
| [<span data-ttu-id="0ffa5-117">Создание Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="0ffa5-117">Create publishedResource</span></span>](../api/publishedresource-post.md) |  [<span data-ttu-id="0ffa5-118">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="0ffa5-118">publishedResource</span></span>](publishedresource.md)  | <span data-ttu-id="0ffa5-119">Создание нового **публишедресаурце**.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-119">Create a new **publishedResource**.</span></span> |
| [<span data-ttu-id="0ffa5-120">Обновление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="0ffa5-120">Update publishedResource</span></span>](../api/publishedresource-update.md) | [<span data-ttu-id="0ffa5-121">публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="0ffa5-121">publishedResource</span></span>](publishedresource.md) | <span data-ttu-id="0ffa5-122">Обновление объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="0ffa5-122">Update a **publishedResource** object.</span></span> |
| [<span data-ttu-id="0ffa5-123">Удаление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="0ffa5-123">Delete  publishedResource</span></span>](../api/publishedresource-delete.md) | <span data-ttu-id="0ffa5-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0ffa5-124">None</span></span> | <span data-ttu-id="0ffa5-125">Удаление объекта **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="0ffa5-125">Delete a **publishedResource** object.</span></span> |
| [<span data-ttu-id="0ffa5-126">Назначение Публишедресаурце для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="0ffa5-126">Assign publishedResource to onPremisesAgentGroup</span></span>](../api/publishedresource-post-agentgroups.md) | <span data-ttu-id="0ffa5-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0ffa5-127">None</span></span> | <span data-ttu-id="0ffa5-128">Назначьте объект **публишедресаурце** для **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-128">Assign a **publishedResource** object to an **onPremisesAgentGroup**.</span></span> |
| [<span data-ttu-id="0ffa5-129">Удаление Публишедресаурце из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="0ffa5-129">Remove publishedResource from onPremisesAgentGroup</span></span>](../api/publishedresource-delete-agentgroups.md) | <span data-ttu-id="0ffa5-130">Нет</span><span class="sxs-lookup"><span data-stu-id="0ffa5-130">None</span></span> |  <span data-ttu-id="0ffa5-131">Удаление объекта **публишедресаурце** из объекта **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-131">Remove a **publishedResource** object from an **onPremisesAgentGroup**.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ffa5-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ffa5-132">Properties</span></span>

| <span data-ttu-id="0ffa5-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ffa5-133">Property</span></span>     | <span data-ttu-id="0ffa5-134">Тип</span><span class="sxs-lookup"><span data-stu-id="0ffa5-134">Type</span></span>        | <span data-ttu-id="0ffa5-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0ffa5-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ffa5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0ffa5-136">displayName</span></span>|<span data-ttu-id="0ffa5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0ffa5-137">String</span></span>| <span data-ttu-id="0ffa5-138">Отображаемое имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-138">Display Name of the publishedResource.</span></span>|
|<span data-ttu-id="0ffa5-139">id</span><span class="sxs-lookup"><span data-stu-id="0ffa5-139">id</span></span>|<span data-ttu-id="0ffa5-140">String</span><span class="sxs-lookup"><span data-stu-id="0ffa5-140">String</span></span>| <span data-ttu-id="0ffa5-141">Идентификатор объекта Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-141">The object id of the publishedResource.</span></span> <span data-ttu-id="0ffa5-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-142">Read-only.</span></span>|
|<span data-ttu-id="0ffa5-143">публишингтипе</span><span class="sxs-lookup"><span data-stu-id="0ffa5-143">publishingType</span></span>|<span data-ttu-id="0ffa5-144">string</span><span class="sxs-lookup"><span data-stu-id="0ffa5-144">string</span></span>| <span data-ttu-id="0ffa5-145">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-145">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|
|<span data-ttu-id="0ffa5-146">resourceName</span><span class="sxs-lookup"><span data-stu-id="0ffa5-146">resourceName</span></span>|<span data-ttu-id="0ffa5-147">String</span><span class="sxs-lookup"><span data-stu-id="0ffa5-147">String</span></span>|<span data-ttu-id="0ffa5-148">Имя Публишедресаурце.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-148">Name of the publishedResource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ffa5-149">Связи</span><span class="sxs-lookup"><span data-stu-id="0ffa5-149">Relationships</span></span>

| <span data-ttu-id="0ffa5-150">Связь</span><span class="sxs-lookup"><span data-stu-id="0ffa5-150">Relationship</span></span> | <span data-ttu-id="0ffa5-151">Тип</span><span class="sxs-lookup"><span data-stu-id="0ffa5-151">Type</span></span>        | <span data-ttu-id="0ffa5-152">Описание</span><span class="sxs-lookup"><span data-stu-id="0ffa5-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ffa5-153">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="0ffa5-153">agentGroups</span></span>|<span data-ttu-id="0ffa5-154">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0ffa5-154">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="0ffa5-155">Список **онпремисесажентграупс** , которым назначено **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="0ffa5-155">List of **onPremisesAgentGroups** that a **publishedResource** is assigned to.</span></span> <span data-ttu-id="0ffa5-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-156">Read-only.</span></span> <span data-ttu-id="0ffa5-157">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-157">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ffa5-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ffa5-158">JSON representation</span></span>

<span data-ttu-id="0ffa5-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ffa5-159">The following is a JSON representation of the resource.</span></span>

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
