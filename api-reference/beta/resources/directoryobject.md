---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5bc558f92b4c812f95f7a859dbfea6a43a2fe33b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973849"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="2ce35-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="2ce35-104">directoryObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ce35-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="2ce35-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="2ce35-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="2ce35-107">This resource supports:</span></span>

- <span data-ttu-id="2ce35-108">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryobject-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="2ce35-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="2ce35-109">Методы</span><span class="sxs-lookup"><span data-stu-id="2ce35-109">Methods</span></span>

| <span data-ttu-id="2ce35-110">Метод</span><span class="sxs-lookup"><span data-stu-id="2ce35-110">Method</span></span>       | <span data-ttu-id="2ce35-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2ce35-111">Return Type</span></span>  |<span data-ttu-id="2ce35-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2ce35-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ce35-113">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="2ce35-113">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="2ce35-114">directoryObject</span><span class="sxs-lookup"><span data-stu-id="2ce35-114">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="2ce35-115">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="2ce35-115">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="2ce35-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="2ce35-116">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="2ce35-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2ce35-117">None</span></span> |<span data-ttu-id="2ce35-118">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="2ce35-118">Delete a directory object.</span></span> |
|[<span data-ttu-id="2ce35-119">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2ce35-119">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="2ce35-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ce35-120">String collection</span></span>|<span data-ttu-id="2ce35-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="2ce35-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="2ce35-123">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2ce35-123">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="2ce35-124">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ce35-124">String collection</span></span>|<span data-ttu-id="2ce35-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="2ce35-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="2ce35-127">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="2ce35-127">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="2ce35-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2ce35-128">String collection</span></span>| <span data-ttu-id="2ce35-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="2ce35-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="2ce35-131">getByIds</span><span class="sxs-lookup"><span data-stu-id="2ce35-131">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="2ce35-132">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2ce35-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="2ce35-133">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="2ce35-133">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="2ce35-134">validateProperties</span><span class="sxs-lookup"><span data-stu-id="2ce35-134">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="2ce35-135">Json</span><span class="sxs-lookup"><span data-stu-id="2ce35-135">Json</span></span>| <span data-ttu-id="2ce35-136">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="2ce35-136">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="2ce35-137">delta</span><span class="sxs-lookup"><span data-stu-id="2ce35-137">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="2ce35-138">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2ce35-138">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="2ce35-139">Получение добавочных изменений для объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="2ce35-139">Get incremental changes for directory objects.</span></span> <span data-ttu-id="2ce35-140">Поддерживает фильтрацию по производному типу.</span><span class="sxs-lookup"><span data-stu-id="2ce35-140">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="2ce35-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ce35-141">Properties</span></span>

| <span data-ttu-id="2ce35-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ce35-142">Property</span></span>   | <span data-ttu-id="2ce35-143">Тип</span><span class="sxs-lookup"><span data-stu-id="2ce35-143">Type</span></span> |<span data-ttu-id="2ce35-144">Описание</span><span class="sxs-lookup"><span data-stu-id="2ce35-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ce35-145">id</span><span class="sxs-lookup"><span data-stu-id="2ce35-145">id</span></span>|<span data-ttu-id="2ce35-146">String</span><span class="sxs-lookup"><span data-stu-id="2ce35-146">String</span></span>|<span data-ttu-id="2ce35-147">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="2ce35-147">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="2ce35-148">Ключ.</span><span class="sxs-lookup"><span data-stu-id="2ce35-148">Key.</span></span> <span data-ttu-id="2ce35-149">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="2ce35-149">Not nullable.</span></span> <span data-ttu-id="2ce35-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce35-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ce35-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="2ce35-151">Relationships</span></span>

<span data-ttu-id="2ce35-152">Нет</span><span class="sxs-lookup"><span data-stu-id="2ce35-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ce35-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ce35-153">JSON representation</span></span>

<span data-ttu-id="2ce35-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ce35-154">Here is a JSON representation of the resource</span></span>

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
