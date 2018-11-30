---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
ms.openlocfilehash: 0981584bb86b71d06e29de4efc379c84bacac51d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028110"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="18dbf-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="18dbf-104">directoryObject resource type</span></span>

<span data-ttu-id="18dbf-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="18dbf-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="18dbf-107">Методы</span><span class="sxs-lookup"><span data-stu-id="18dbf-107">Methods</span></span>

| <span data-ttu-id="18dbf-108">Метод</span><span class="sxs-lookup"><span data-stu-id="18dbf-108">Method</span></span>       | <span data-ttu-id="18dbf-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18dbf-109">Return Type</span></span>  |<span data-ttu-id="18dbf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="18dbf-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18dbf-111">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="18dbf-111">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="18dbf-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="18dbf-112">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="18dbf-113">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="18dbf-113">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="18dbf-114">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="18dbf-114">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="18dbf-115">Нет</span><span class="sxs-lookup"><span data-stu-id="18dbf-115">None</span></span> |<span data-ttu-id="18dbf-116">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="18dbf-116">Delete a directory object.</span></span> |
|[<span data-ttu-id="18dbf-117">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="18dbf-117">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="18dbf-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="18dbf-118">String collection</span></span>|<span data-ttu-id="18dbf-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="18dbf-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="18dbf-121">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="18dbf-121">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="18dbf-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="18dbf-122">String collection</span></span>|<span data-ttu-id="18dbf-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="18dbf-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="18dbf-125">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="18dbf-125">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="18dbf-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="18dbf-126">String collection</span></span>| <span data-ttu-id="18dbf-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="18dbf-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="18dbf-129">getByIds</span><span class="sxs-lookup"><span data-stu-id="18dbf-129">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="18dbf-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="18dbf-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="18dbf-131">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="18dbf-131">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="18dbf-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="18dbf-132">Properties</span></span>

| <span data-ttu-id="18dbf-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="18dbf-133">Property</span></span>   | <span data-ttu-id="18dbf-134">Тип</span><span class="sxs-lookup"><span data-stu-id="18dbf-134">Type</span></span> |<span data-ttu-id="18dbf-135">Описание</span><span class="sxs-lookup"><span data-stu-id="18dbf-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18dbf-136">id</span><span class="sxs-lookup"><span data-stu-id="18dbf-136">id</span></span>|<span data-ttu-id="18dbf-137">String</span><span class="sxs-lookup"><span data-stu-id="18dbf-137">String</span></span>|<span data-ttu-id="18dbf-p106">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18dbf-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18dbf-142">Связи</span><span class="sxs-lookup"><span data-stu-id="18dbf-142">Relationships</span></span>

<span data-ttu-id="18dbf-143">Нет</span><span class="sxs-lookup"><span data-stu-id="18dbf-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="18dbf-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18dbf-144">JSON representation</span></span>

<span data-ttu-id="18dbf-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18dbf-145">Here is a JSON representation of the resource</span></span>

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
