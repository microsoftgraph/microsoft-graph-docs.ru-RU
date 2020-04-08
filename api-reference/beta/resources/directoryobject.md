---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 43fd850274006d763535ad30b2de58f634375541
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181696"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="f12fd-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="f12fd-104">directoryObject resource type</span></span>

<span data-ttu-id="f12fd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f12fd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f12fd-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="f12fd-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="f12fd-108">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="f12fd-108">This resource supports:</span></span>

- <span data-ttu-id="f12fd-109">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryobject-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="f12fd-109">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="f12fd-110">Методы</span><span class="sxs-lookup"><span data-stu-id="f12fd-110">Methods</span></span>

| <span data-ttu-id="f12fd-111">Метод</span><span class="sxs-lookup"><span data-stu-id="f12fd-111">Method</span></span>       | <span data-ttu-id="f12fd-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f12fd-112">Return Type</span></span>  |<span data-ttu-id="f12fd-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f12fd-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f12fd-114">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="f12fd-114">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="f12fd-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="f12fd-115">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="f12fd-116">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="f12fd-116">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="f12fd-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="f12fd-117">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="f12fd-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f12fd-118">None</span></span> |<span data-ttu-id="f12fd-119">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="f12fd-119">Delete a directory object.</span></span> |
|[<span data-ttu-id="f12fd-120">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f12fd-120">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="f12fd-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f12fd-121">String collection</span></span>|<span data-ttu-id="f12fd-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="f12fd-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="f12fd-124">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f12fd-124">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="f12fd-125">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f12fd-125">String collection</span></span>|<span data-ttu-id="f12fd-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="f12fd-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="f12fd-128">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="f12fd-128">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="f12fd-129">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f12fd-129">String collection</span></span>| <span data-ttu-id="f12fd-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="f12fd-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="f12fd-132">getByIds</span><span class="sxs-lookup"><span data-stu-id="f12fd-132">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="f12fd-133">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="f12fd-133">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="f12fd-134">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="f12fd-134">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="f12fd-135">validateProperties</span><span class="sxs-lookup"><span data-stu-id="f12fd-135">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="f12fd-136">Json</span><span class="sxs-lookup"><span data-stu-id="f12fd-136">Json</span></span>| <span data-ttu-id="f12fd-137">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="f12fd-137">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="f12fd-138">delta</span><span class="sxs-lookup"><span data-stu-id="f12fd-138">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="f12fd-139">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="f12fd-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="f12fd-140">Получение добавочных изменений для объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="f12fd-140">Get incremental changes for directory objects.</span></span> <span data-ttu-id="f12fd-141">Поддерживает фильтрацию по производному типу.</span><span class="sxs-lookup"><span data-stu-id="f12fd-141">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="f12fd-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="f12fd-142">Properties</span></span>

| <span data-ttu-id="f12fd-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="f12fd-143">Property</span></span>   | <span data-ttu-id="f12fd-144">Тип</span><span class="sxs-lookup"><span data-stu-id="f12fd-144">Type</span></span> |<span data-ttu-id="f12fd-145">Описание</span><span class="sxs-lookup"><span data-stu-id="f12fd-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f12fd-146">id</span><span class="sxs-lookup"><span data-stu-id="f12fd-146">id</span></span>|<span data-ttu-id="f12fd-147">String</span><span class="sxs-lookup"><span data-stu-id="f12fd-147">String</span></span>|<span data-ttu-id="f12fd-148">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="f12fd-148">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="f12fd-149">Ключ.</span><span class="sxs-lookup"><span data-stu-id="f12fd-149">Key.</span></span> <span data-ttu-id="f12fd-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="f12fd-150">Not nullable.</span></span> <span data-ttu-id="f12fd-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f12fd-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f12fd-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="f12fd-152">Relationships</span></span>

<span data-ttu-id="f12fd-153">Нет</span><span class="sxs-lookup"><span data-stu-id="f12fd-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f12fd-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f12fd-154">JSON representation</span></span>

<span data-ttu-id="f12fd-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f12fd-155">Here is a JSON representation of the resource</span></span>

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
