---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
ms.openlocfilehash: ed49c042ab9456479d0f9f7fee49a72a93767e81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082010"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="73132-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="73132-104">directoryObject resource type</span></span>

> <span data-ttu-id="73132-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73132-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73132-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73132-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73132-p103">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="73132-p103">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="73132-109">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="73132-109">This resource supports:</span></span>

- <span data-ttu-id="73132-110">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryobject-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="73132-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="73132-111">Методы</span><span class="sxs-lookup"><span data-stu-id="73132-111">Methods</span></span>

| <span data-ttu-id="73132-112">Метод</span><span class="sxs-lookup"><span data-stu-id="73132-112">Method</span></span>       | <span data-ttu-id="73132-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="73132-113">Return Type</span></span>  |<span data-ttu-id="73132-114">Описание</span><span class="sxs-lookup"><span data-stu-id="73132-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73132-115">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="73132-115">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="73132-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="73132-116">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="73132-117">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="73132-117">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="73132-118">Delete</span><span class="sxs-lookup"><span data-stu-id="73132-118">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="73132-119">Нет</span><span class="sxs-lookup"><span data-stu-id="73132-119">None</span></span> |<span data-ttu-id="73132-120">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="73132-120">Delete a directory object.</span></span> |
|[<span data-ttu-id="73132-121">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="73132-121">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="73132-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="73132-122">String collection</span></span>|<span data-ttu-id="73132-p104">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="73132-p104">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="73132-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="73132-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="73132-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="73132-126">String collection</span></span>|<span data-ttu-id="73132-p105">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="73132-p105">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="73132-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="73132-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="73132-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="73132-130">String collection</span></span>| <span data-ttu-id="73132-p106">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="73132-p106">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="73132-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="73132-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="73132-134">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="73132-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="73132-135">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="73132-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="73132-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="73132-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="73132-137">JSON</span><span class="sxs-lookup"><span data-stu-id="73132-137">JSON</span></span>| <span data-ttu-id="73132-138">Проверить группу Office 365 отображаемое имя или псевдоним почты стандарту именования политик.</span><span class="sxs-lookup"><span data-stu-id="73132-138">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="73132-139">delta</span><span class="sxs-lookup"><span data-stu-id="73132-139">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="73132-140">Коллекция directoryObject</span><span class="sxs-lookup"><span data-stu-id="73132-140">directoryObject collection</span></span>| <span data-ttu-id="73132-141">Получите добавочные изменения объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="73132-141">Get incremental changes for directory objects.</span></span> <span data-ttu-id="73132-142">Поддерживает фильтрацию по типу производные.</span><span class="sxs-lookup"><span data-stu-id="73132-142">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="73132-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="73132-143">Properties</span></span>

| <span data-ttu-id="73132-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="73132-144">Property</span></span>   | <span data-ttu-id="73132-145">Тип</span><span class="sxs-lookup"><span data-stu-id="73132-145">Type</span></span> |<span data-ttu-id="73132-146">Описание</span><span class="sxs-lookup"><span data-stu-id="73132-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73132-147">id</span><span class="sxs-lookup"><span data-stu-id="73132-147">id</span></span>|<span data-ttu-id="73132-148">String</span><span class="sxs-lookup"><span data-stu-id="73132-148">String</span></span>|<span data-ttu-id="73132-149">Идентификатор Guid, который является уникальный идентификатор для объекта. например 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="73132-149">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="73132-150">Ключ.</span><span class="sxs-lookup"><span data-stu-id="73132-150">Key.</span></span> <span data-ttu-id="73132-151">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="73132-151">Not nullable.</span></span> <span data-ttu-id="73132-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="73132-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73132-153">Связи</span><span class="sxs-lookup"><span data-stu-id="73132-153">Relationships</span></span>

<span data-ttu-id="73132-154">Нет</span><span class="sxs-lookup"><span data-stu-id="73132-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73132-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73132-155">JSON representation</span></span>

<span data-ttu-id="73132-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73132-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
