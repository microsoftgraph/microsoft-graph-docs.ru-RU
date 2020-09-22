---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ae5c016bcc6ccb317a56b1d248c8450703d5d34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013853"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="fc0c3-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="fc0c3-104">directoryObject resource type</span></span>

<span data-ttu-id="fc0c3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc0c3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc0c3-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="fc0c3-108">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="fc0c3-108">This resource supports:</span></span>

- <span data-ttu-id="fc0c3-109">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryobject-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="fc0c3-109">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="fc0c3-110">Методы</span><span class="sxs-lookup"><span data-stu-id="fc0c3-110">Methods</span></span>

| <span data-ttu-id="fc0c3-111">Метод</span><span class="sxs-lookup"><span data-stu-id="fc0c3-111">Method</span></span>       | <span data-ttu-id="fc0c3-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc0c3-112">Return Type</span></span>  |<span data-ttu-id="fc0c3-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fc0c3-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc0c3-114">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="fc0c3-114">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="fc0c3-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fc0c3-115">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="fc0c3-116">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-116">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="fc0c3-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="fc0c3-117">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="fc0c3-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fc0c3-118">None</span></span> |<span data-ttu-id="fc0c3-119">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-119">Delete a directory object.</span></span> |
|[<span data-ttu-id="fc0c3-120">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="fc0c3-120">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="fc0c3-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc0c3-121">String collection</span></span>|<span data-ttu-id="fc0c3-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="fc0c3-124">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="fc0c3-124">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="fc0c3-125">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc0c3-125">String collection</span></span>|<span data-ttu-id="fc0c3-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="fc0c3-128">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="fc0c3-128">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="fc0c3-129">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc0c3-129">String collection</span></span>| <span data-ttu-id="fc0c3-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="fc0c3-132">getByIds</span><span class="sxs-lookup"><span data-stu-id="fc0c3-132">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="fc0c3-133">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fc0c3-133">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="fc0c3-134">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-134">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="fc0c3-135">validateProperties</span><span class="sxs-lookup"><span data-stu-id="fc0c3-135">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="fc0c3-136">Json</span><span class="sxs-lookup"><span data-stu-id="fc0c3-136">Json</span></span>| <span data-ttu-id="fc0c3-137">Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-137">Validate a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="fc0c3-138">delta</span><span class="sxs-lookup"><span data-stu-id="fc0c3-138">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="fc0c3-139">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fc0c3-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="fc0c3-140">Получение добавочных изменений для объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-140">Get incremental changes for directory objects.</span></span> <span data-ttu-id="fc0c3-141">Поддерживает фильтрацию по производному типу.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-141">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc0c3-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc0c3-142">Properties</span></span>

| <span data-ttu-id="fc0c3-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc0c3-143">Property</span></span>   | <span data-ttu-id="fc0c3-144">Тип</span><span class="sxs-lookup"><span data-stu-id="fc0c3-144">Type</span></span> |<span data-ttu-id="fc0c3-145">Описание</span><span class="sxs-lookup"><span data-stu-id="fc0c3-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc0c3-146">id</span><span class="sxs-lookup"><span data-stu-id="fc0c3-146">id</span></span>|<span data-ttu-id="fc0c3-147">String</span><span class="sxs-lookup"><span data-stu-id="fc0c3-147">String</span></span>|<span data-ttu-id="fc0c3-148">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-148">The unique identifier for the object.</span></span> <span data-ttu-id="fc0c3-149">Например, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-149">For example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="fc0c3-150">Значение свойства **идентификатор**оформлено часто, но не только в виде GUID; необходимо считать его непрозрачным идентификатором и не полагаться на то, что он является GUID.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-150">The value of the **id** property is often but not exclusively in the form of a GUID; treat it as an opaque identifier and do not rely on it being a GUID.</span></span> <span data-ttu-id="fc0c3-151">Ключ.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-151">Key.</span></span> <span data-ttu-id="fc0c3-152">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-152">Not nullable.</span></span> <span data-ttu-id="fc0c3-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-153">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc0c3-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="fc0c3-154">Relationships</span></span>

<span data-ttu-id="fc0c3-155">Нет</span><span class="sxs-lookup"><span data-stu-id="fc0c3-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc0c3-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc0c3-156">JSON representation</span></span>

<span data-ttu-id="fc0c3-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc0c3-157">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "openType": true
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


