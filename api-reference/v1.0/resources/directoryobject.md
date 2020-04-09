---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8014c238487d5ada0f05f1a6edfed0402b25ae1a
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181869"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="c3d8f-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="c3d8f-104">directoryObject resource type</span></span>

<span data-ttu-id="c3d8f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3d8f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c3d8f-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="c3d8f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c3d8f-108">Methods</span></span>

| <span data-ttu-id="c3d8f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c3d8f-109">Method</span></span>       | <span data-ttu-id="c3d8f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3d8f-110">Return Type</span></span>  |<span data-ttu-id="c3d8f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3d8f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3d8f-112">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="c3d8f-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="c3d8f-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c3d8f-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="c3d8f-114">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="c3d8f-115">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="c3d8f-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="c3d8f-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c3d8f-116">None</span></span> |<span data-ttu-id="c3d8f-117">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="c3d8f-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="c3d8f-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="c3d8f-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3d8f-119">String collection</span></span>|<span data-ttu-id="c3d8f-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="c3d8f-122">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="c3d8f-122">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="c3d8f-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3d8f-123">String collection</span></span>|<span data-ttu-id="c3d8f-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="c3d8f-126">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="c3d8f-126">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="c3d8f-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3d8f-127">String collection</span></span>| <span data-ttu-id="c3d8f-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="c3d8f-130">getByIds</span><span class="sxs-lookup"><span data-stu-id="c3d8f-130">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="c3d8f-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c3d8f-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="c3d8f-132">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-132">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="c3d8f-133">validateProperties</span><span class="sxs-lookup"><span data-stu-id="c3d8f-133">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="c3d8f-134">Json</span><span class="sxs-lookup"><span data-stu-id="c3d8f-134">Json</span></span>| <span data-ttu-id="c3d8f-135">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-135">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="c3d8f-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3d8f-136">Properties</span></span>

| <span data-ttu-id="c3d8f-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3d8f-137">Property</span></span>   | <span data-ttu-id="c3d8f-138">Тип</span><span class="sxs-lookup"><span data-stu-id="c3d8f-138">Type</span></span> |<span data-ttu-id="c3d8f-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c3d8f-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3d8f-140">id</span><span class="sxs-lookup"><span data-stu-id="c3d8f-140">id</span></span>|<span data-ttu-id="c3d8f-141">String</span><span class="sxs-lookup"><span data-stu-id="c3d8f-141">String</span></span>|<span data-ttu-id="c3d8f-p106">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3d8f-146">Связи</span><span class="sxs-lookup"><span data-stu-id="c3d8f-146">Relationships</span></span>

<span data-ttu-id="c3d8f-147">Нет</span><span class="sxs-lookup"><span data-stu-id="c3d8f-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c3d8f-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3d8f-148">JSON representation</span></span>

<span data-ttu-id="c3d8f-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3d8f-149">Here is a JSON representation of the resource</span></span>

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
