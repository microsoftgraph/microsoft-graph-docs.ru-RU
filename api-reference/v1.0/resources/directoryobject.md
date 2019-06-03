---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b71de12ba6a0053cd97749fd72dc22f7ab961539
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34658031"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="e9e73-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9e73-104">directoryObject resource type</span></span>

<span data-ttu-id="e9e73-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="e9e73-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="e9e73-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e9e73-107">Methods</span></span>

| <span data-ttu-id="e9e73-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e9e73-108">Method</span></span>       | <span data-ttu-id="e9e73-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e9e73-109">Return Type</span></span>  |<span data-ttu-id="e9e73-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e73-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e9e73-111">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9e73-111">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="e9e73-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9e73-112">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="e9e73-113">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="e9e73-113">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="e9e73-114">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9e73-114">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="e9e73-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e9e73-115">None</span></span> |<span data-ttu-id="e9e73-116">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="e9e73-116">Delete a directory object.</span></span> |
|[<span data-ttu-id="e9e73-117">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e9e73-117">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="e9e73-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9e73-118">String collection</span></span>|<span data-ttu-id="e9e73-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="e9e73-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="e9e73-121">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e9e73-121">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="e9e73-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9e73-122">String collection</span></span>|<span data-ttu-id="e9e73-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="e9e73-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="e9e73-125">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="e9e73-125">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="e9e73-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9e73-126">String collection</span></span>| <span data-ttu-id="e9e73-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="e9e73-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="e9e73-129">getByIds</span><span class="sxs-lookup"><span data-stu-id="e9e73-129">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="e9e73-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e9e73-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e9e73-131">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="e9e73-131">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="e9e73-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9e73-132">Properties</span></span>

| <span data-ttu-id="e9e73-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9e73-133">Property</span></span>   | <span data-ttu-id="e9e73-134">Тип</span><span class="sxs-lookup"><span data-stu-id="e9e73-134">Type</span></span> |<span data-ttu-id="e9e73-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e73-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9e73-136">id</span><span class="sxs-lookup"><span data-stu-id="e9e73-136">id</span></span>|<span data-ttu-id="e9e73-137">String</span><span class="sxs-lookup"><span data-stu-id="e9e73-137">String</span></span>|<span data-ttu-id="e9e73-p106">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9e73-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9e73-142">Связи</span><span class="sxs-lookup"><span data-stu-id="e9e73-142">Relationships</span></span>

<span data-ttu-id="e9e73-143">Нет</span><span class="sxs-lookup"><span data-stu-id="e9e73-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e9e73-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9e73-144">JSON representation</span></span>

<span data-ttu-id="e9e73-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9e73-145">Here is a JSON representation of the resource</span></span>

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
