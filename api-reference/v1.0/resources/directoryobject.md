---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 01548a3f1be4725fad1814f4a509a13a987858e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531652"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="b1681-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="b1681-104">directoryObject resource type</span></span>

<span data-ttu-id="b1681-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1681-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1681-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="b1681-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="b1681-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b1681-108">Methods</span></span>

| <span data-ttu-id="b1681-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b1681-109">Method</span></span>       | <span data-ttu-id="b1681-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b1681-110">Return Type</span></span>  |<span data-ttu-id="b1681-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b1681-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1681-112">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="b1681-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="b1681-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="b1681-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="b1681-114">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="b1681-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="b1681-115">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="b1681-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="b1681-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b1681-116">None</span></span> |<span data-ttu-id="b1681-117">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="b1681-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="b1681-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b1681-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="b1681-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1681-119">String collection</span></span>|<span data-ttu-id="b1681-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="b1681-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="b1681-122">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b1681-122">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="b1681-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1681-123">String collection</span></span>|<span data-ttu-id="b1681-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="b1681-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="b1681-126">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b1681-126">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="b1681-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1681-127">String collection</span></span>| <span data-ttu-id="b1681-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="b1681-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="b1681-130">getByIds</span><span class="sxs-lookup"><span data-stu-id="b1681-130">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="b1681-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="b1681-131">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b1681-132">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="b1681-132">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="b1681-133">validateProperties</span><span class="sxs-lookup"><span data-stu-id="b1681-133">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="b1681-134">Json</span><span class="sxs-lookup"><span data-stu-id="b1681-134">Json</span></span>| <span data-ttu-id="b1681-135">Проверка соответствия отображаемого имени или почтового псевдонима группы Office 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="b1681-135">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="b1681-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1681-136">Properties</span></span>

| <span data-ttu-id="b1681-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1681-137">Property</span></span>   | <span data-ttu-id="b1681-138">Тип</span><span class="sxs-lookup"><span data-stu-id="b1681-138">Type</span></span> |<span data-ttu-id="b1681-139">Описание</span><span class="sxs-lookup"><span data-stu-id="b1681-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1681-140">id</span><span class="sxs-lookup"><span data-stu-id="b1681-140">id</span></span>|<span data-ttu-id="b1681-141">String</span><span class="sxs-lookup"><span data-stu-id="b1681-141">String</span></span>|<span data-ttu-id="b1681-p106">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1681-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1681-146">Связи</span><span class="sxs-lookup"><span data-stu-id="b1681-146">Relationships</span></span>

<span data-ttu-id="b1681-147">Нет</span><span class="sxs-lookup"><span data-stu-id="b1681-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1681-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1681-148">JSON representation</span></span>

<span data-ttu-id="b1681-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1681-149">Here is a JSON representation of the resource</span></span>

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
