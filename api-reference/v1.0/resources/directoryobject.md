---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 83750686b4075f7577e88e1e6107dd2f2a5f4d2f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439907"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="3f94c-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="3f94c-104">directoryObject resource type</span></span>

<span data-ttu-id="3f94c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f94c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f94c-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="3f94c-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="3f94c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="3f94c-108">Methods</span></span>

| <span data-ttu-id="3f94c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="3f94c-109">Method</span></span>       | <span data-ttu-id="3f94c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3f94c-110">Return Type</span></span>  |<span data-ttu-id="3f94c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3f94c-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f94c-112">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="3f94c-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="3f94c-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="3f94c-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="3f94c-114">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="3f94c-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="3f94c-115">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="3f94c-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="3f94c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3f94c-116">None</span></span> |<span data-ttu-id="3f94c-117">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="3f94c-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="3f94c-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="3f94c-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="3f94c-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f94c-119">String collection</span></span>|<span data-ttu-id="3f94c-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="3f94c-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="3f94c-122">Получение доступных свойств расширения</span><span class="sxs-lookup"><span data-stu-id="3f94c-122">Get available extension properties</span></span>](../api/directoryobject-getavailableextensionproperties.md)|<span data-ttu-id="3f94c-123">Коллекция [extensionProperty](../resources/extensionproperty.md)</span><span class="sxs-lookup"><span data-stu-id="3f94c-123">[extensionProperty](../resources/extensionproperty.md) collection</span></span>|<span data-ttu-id="3f94c-124">Получение полного или отфильтрованного списка свойств расширения каталога, которые зарегистрированы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="3f94c-124">Get all or a filtered list of the directory extension properties that have been registered in a directory.</span></span>|
|[<span data-ttu-id="3f94c-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="3f94c-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="3f94c-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f94c-126">String collection</span></span>|<span data-ttu-id="3f94c-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="3f94c-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="3f94c-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="3f94c-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="3f94c-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f94c-130">String collection</span></span>| <span data-ttu-id="3f94c-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="3f94c-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="3f94c-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="3f94c-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="3f94c-134">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3f94c-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="3f94c-135">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="3f94c-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="3f94c-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="3f94c-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="3f94c-137">Json</span><span class="sxs-lookup"><span data-stu-id="3f94c-137">Json</span></span>| <span data-ttu-id="3f94c-138">Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="3f94c-138">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="3f94c-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f94c-139">Properties</span></span>

| <span data-ttu-id="3f94c-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f94c-140">Property</span></span>   | <span data-ttu-id="3f94c-141">Тип</span><span class="sxs-lookup"><span data-stu-id="3f94c-141">Type</span></span> |<span data-ttu-id="3f94c-142">Описание</span><span class="sxs-lookup"><span data-stu-id="3f94c-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f94c-143">id</span><span class="sxs-lookup"><span data-stu-id="3f94c-143">id</span></span>|<span data-ttu-id="3f94c-144">String</span><span class="sxs-lookup"><span data-stu-id="3f94c-144">String</span></span>|<span data-ttu-id="3f94c-145">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="3f94c-145">The unique identifier for the object.</span></span> <span data-ttu-id="3f94c-146">Например, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="3f94c-146">For example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="3f94c-147">Значение свойства **идентификатор** оформлено часто, но не только в виде GUID; необходимо считать его непрозрачным идентификатором и не полагаться на то, что он является GUID.</span><span class="sxs-lookup"><span data-stu-id="3f94c-147">The value of the **id** property is often but not exclusively in the form of a GUID; treat it as an opaque identifier and do not rely on it being a GUID.</span></span> <span data-ttu-id="3f94c-148">Ключ.</span><span class="sxs-lookup"><span data-stu-id="3f94c-148">Key.</span></span> <span data-ttu-id="3f94c-149">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="3f94c-149">Not nullable.</span></span> <span data-ttu-id="3f94c-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f94c-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f94c-151">Связи</span><span class="sxs-lookup"><span data-stu-id="3f94c-151">Relationships</span></span>

<span data-ttu-id="3f94c-152">Нет</span><span class="sxs-lookup"><span data-stu-id="3f94c-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3f94c-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f94c-153">JSON representation</span></span>

<span data-ttu-id="3f94c-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f94c-154">Here is a JSON representation of the resource</span></span>

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

