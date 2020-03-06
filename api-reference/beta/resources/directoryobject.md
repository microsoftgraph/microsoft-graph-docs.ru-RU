---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b90e81a9337cef51af4bfded50eaaf494e4ebca7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507032"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="9fdb5-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="9fdb5-104">directoryObject resource type</span></span>

<span data-ttu-id="9fdb5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fdb5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fdb5-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="9fdb5-108">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="9fdb5-108">This resource supports:</span></span>

- <span data-ttu-id="9fdb5-109">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryobject-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="9fdb5-109">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="9fdb5-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9fdb5-110">Methods</span></span>

| <span data-ttu-id="9fdb5-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9fdb5-111">Method</span></span>       | <span data-ttu-id="9fdb5-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9fdb5-112">Return Type</span></span>  |<span data-ttu-id="9fdb5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9fdb5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fdb5-114">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="9fdb5-114">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="9fdb5-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9fdb5-115">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="9fdb5-116">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-116">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="9fdb5-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="9fdb5-117">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="9fdb5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9fdb5-118">None</span></span> |<span data-ttu-id="9fdb5-119">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-119">Delete a directory object.</span></span> |
|[<span data-ttu-id="9fdb5-120">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9fdb5-120">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="9fdb5-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9fdb5-121">String collection</span></span>|<span data-ttu-id="9fdb5-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="9fdb5-124">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9fdb5-124">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="9fdb5-125">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9fdb5-125">String collection</span></span>|<span data-ttu-id="9fdb5-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="9fdb5-128">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="9fdb5-128">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="9fdb5-129">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9fdb5-129">String collection</span></span>| <span data-ttu-id="9fdb5-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="9fdb5-132">getByIds</span><span class="sxs-lookup"><span data-stu-id="9fdb5-132">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="9fdb5-133">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9fdb5-133">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="9fdb5-134">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-134">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="9fdb5-135">validateProperties</span><span class="sxs-lookup"><span data-stu-id="9fdb5-135">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="9fdb5-136">Json</span><span class="sxs-lookup"><span data-stu-id="9fdb5-136">Json</span></span>| <span data-ttu-id="9fdb5-137">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-137">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="9fdb5-138">delta</span><span class="sxs-lookup"><span data-stu-id="9fdb5-138">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="9fdb5-139">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9fdb5-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9fdb5-140">Получение добавочных изменений для объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-140">Get incremental changes for directory objects.</span></span> <span data-ttu-id="9fdb5-141">Поддерживает фильтрацию по производному типу.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-141">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="9fdb5-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fdb5-142">Properties</span></span>

| <span data-ttu-id="9fdb5-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fdb5-143">Property</span></span>   | <span data-ttu-id="9fdb5-144">Тип</span><span class="sxs-lookup"><span data-stu-id="9fdb5-144">Type</span></span> |<span data-ttu-id="9fdb5-145">Описание</span><span class="sxs-lookup"><span data-stu-id="9fdb5-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fdb5-146">id</span><span class="sxs-lookup"><span data-stu-id="9fdb5-146">id</span></span>|<span data-ttu-id="9fdb5-147">String</span><span class="sxs-lookup"><span data-stu-id="9fdb5-147">String</span></span>|<span data-ttu-id="9fdb5-148">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-148">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="9fdb5-149">Ключ.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-149">Key.</span></span> <span data-ttu-id="9fdb5-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-150">Not nullable.</span></span> <span data-ttu-id="9fdb5-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fdb5-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="9fdb5-152">Relationships</span></span>

<span data-ttu-id="9fdb5-153">Нет</span><span class="sxs-lookup"><span data-stu-id="9fdb5-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fdb5-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fdb5-154">JSON representation</span></span>

<span data-ttu-id="9fdb5-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fdb5-155">Here is a JSON representation of the resource</span></span>

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
