---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87fb1c21e2fa1e9788890d97f6afbd0b494c555e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640569"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="ac310-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="ac310-104">directoryObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac310-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="ac310-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

<span data-ttu-id="ac310-107">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="ac310-107">This resource supports:</span></span>

- <span data-ttu-id="ac310-108">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryobject-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="ac310-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryobject-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="ac310-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ac310-109">Methods</span></span>

| <span data-ttu-id="ac310-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ac310-110">Method</span></span>       | <span data-ttu-id="ac310-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ac310-111">Return Type</span></span>  |<span data-ttu-id="ac310-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ac310-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac310-113">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="ac310-113">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="ac310-114">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ac310-114">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="ac310-115">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="ac310-115">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="ac310-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="ac310-116">Delete</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="ac310-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ac310-117">None</span></span> |<span data-ttu-id="ac310-118">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="ac310-118">Delete a directory object.</span></span> |
|[<span data-ttu-id="ac310-119">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ac310-119">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="ac310-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ac310-120">String collection</span></span>|<span data-ttu-id="ac310-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="ac310-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="ac310-123">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ac310-123">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="ac310-124">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ac310-124">String collection</span></span>|<span data-ttu-id="ac310-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="ac310-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="ac310-127">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="ac310-127">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="ac310-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ac310-128">String collection</span></span>| <span data-ttu-id="ac310-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="ac310-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="ac310-131">getByIds</span><span class="sxs-lookup"><span data-stu-id="ac310-131">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="ac310-132">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ac310-132">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="ac310-133">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="ac310-133">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="ac310-134">validateProperties</span><span class="sxs-lookup"><span data-stu-id="ac310-134">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="ac310-135">JSON</span><span class="sxs-lookup"><span data-stu-id="ac310-135">JSON</span></span>| <span data-ttu-id="ac310-136">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="ac310-136">Validate an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |
|[<span data-ttu-id="ac310-137">delta</span><span class="sxs-lookup"><span data-stu-id="ac310-137">delta</span></span>](../api/directoryobject-delta.md)|<span data-ttu-id="ac310-138">Коллекция directoryObject</span><span class="sxs-lookup"><span data-stu-id="ac310-138">directoryObject collection</span></span>| <span data-ttu-id="ac310-139">Получение добавочных изменений для объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="ac310-139">Get incremental changes for directory objects.</span></span> <span data-ttu-id="ac310-140">Поддерживает фильтрацию по производному типу.</span><span class="sxs-lookup"><span data-stu-id="ac310-140">Supports filtering by derrived type.</span></span> |

## <a name="properties"></a><span data-ttu-id="ac310-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac310-141">Properties</span></span>

| <span data-ttu-id="ac310-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac310-142">Property</span></span>   | <span data-ttu-id="ac310-143">Тип</span><span class="sxs-lookup"><span data-stu-id="ac310-143">Type</span></span> |<span data-ttu-id="ac310-144">Описание</span><span class="sxs-lookup"><span data-stu-id="ac310-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac310-145">id</span><span class="sxs-lookup"><span data-stu-id="ac310-145">id</span></span>|<span data-ttu-id="ac310-146">String</span><span class="sxs-lookup"><span data-stu-id="ac310-146">String</span></span>|<span data-ttu-id="ac310-147">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde12.</span><span class="sxs-lookup"><span data-stu-id="ac310-147">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde12.</span></span> <span data-ttu-id="ac310-148">Ключ.</span><span class="sxs-lookup"><span data-stu-id="ac310-148">Key.</span></span> <span data-ttu-id="ac310-149">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="ac310-149">Not nullable.</span></span> <span data-ttu-id="ac310-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac310-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac310-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="ac310-151">Relationships</span></span>

<span data-ttu-id="ac310-152">Нет</span><span class="sxs-lookup"><span data-stu-id="ac310-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac310-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac310-153">JSON representation</span></span>

<span data-ttu-id="ac310-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac310-154">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
