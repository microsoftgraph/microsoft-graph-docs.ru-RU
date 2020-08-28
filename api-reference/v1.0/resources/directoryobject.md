---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aa0134fdd39c339b2dbeb0a611850971b1a9d0ee
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287451"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="ad523-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="ad523-104">directoryObject resource type</span></span>

<span data-ttu-id="ad523-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad523-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad523-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="ad523-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="ad523-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ad523-108">Methods</span></span>

| <span data-ttu-id="ad523-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ad523-109">Method</span></span>       | <span data-ttu-id="ad523-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ad523-110">Return Type</span></span>  |<span data-ttu-id="ad523-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ad523-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad523-112">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="ad523-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="ad523-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ad523-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="ad523-114">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="ad523-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="ad523-115">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="ad523-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="ad523-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ad523-116">None</span></span> |<span data-ttu-id="ad523-117">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="ad523-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="ad523-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ad523-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="ad523-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ad523-119">String collection</span></span>|<span data-ttu-id="ad523-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="ad523-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="ad523-122">Получение доступных свойств расширения</span><span class="sxs-lookup"><span data-stu-id="ad523-122">Get available extension properties</span></span>](../api/directoryobject-getavailableextensionproperties.md)|<span data-ttu-id="ad523-123">Коллекция [extensionProperty](../resources/extensionproperty.md)</span><span class="sxs-lookup"><span data-stu-id="ad523-123">[extensionProperty](../resources/extensionproperty.md) collection</span></span>|<span data-ttu-id="ad523-124">Получение полного или отфильтрованного списка свойств расширения каталога, которые зарегистрированы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ad523-124">Get all or a filtered list of the directory extension properties that have been registered in a directory.</span></span>|
|[<span data-ttu-id="ad523-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ad523-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="ad523-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ad523-126">String collection</span></span>|<span data-ttu-id="ad523-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="ad523-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="ad523-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="ad523-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="ad523-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ad523-130">String collection</span></span>| <span data-ttu-id="ad523-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="ad523-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="ad523-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="ad523-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="ad523-134">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ad523-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="ad523-135">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="ad523-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="ad523-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="ad523-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="ad523-137">Json</span><span class="sxs-lookup"><span data-stu-id="ad523-137">Json</span></span>| <span data-ttu-id="ad523-138">Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="ad523-138">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="ad523-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad523-139">Properties</span></span>

| <span data-ttu-id="ad523-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad523-140">Property</span></span>   | <span data-ttu-id="ad523-141">Тип</span><span class="sxs-lookup"><span data-stu-id="ad523-141">Type</span></span> |<span data-ttu-id="ad523-142">Описание</span><span class="sxs-lookup"><span data-stu-id="ad523-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad523-143">id</span><span class="sxs-lookup"><span data-stu-id="ad523-143">id</span></span>|<span data-ttu-id="ad523-144">String</span><span class="sxs-lookup"><span data-stu-id="ad523-144">String</span></span>|<span data-ttu-id="ad523-145">Уникальный идентификатор пользователя объекта.</span><span class="sxs-lookup"><span data-stu-id="ad523-145">The unique identifier for the object.</span></span> <span data-ttu-id="ad523-146">Например, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="ad523-146">For example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="ad523-147">Значение свойства **идентификатор** часто, но не только в форме GUID; считать его непрозрачным идентификатором и не полагаться на то, что он является идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="ad523-147">The value of the **id** property is often but not exclusively in the form of a GUID; treat it as an opaque identifier and do not rely on it being a GUID.</span></span> <span data-ttu-id="ad523-148">Ключ.</span><span class="sxs-lookup"><span data-stu-id="ad523-148">Key.</span></span> <span data-ttu-id="ad523-149">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="ad523-149">Not nullable.</span></span> <span data-ttu-id="ad523-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad523-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad523-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="ad523-151">Relationships</span></span>

<span data-ttu-id="ad523-152">Нет</span><span class="sxs-lookup"><span data-stu-id="ad523-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ad523-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad523-153">JSON representation</span></span>

<span data-ttu-id="ad523-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad523-154">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
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
