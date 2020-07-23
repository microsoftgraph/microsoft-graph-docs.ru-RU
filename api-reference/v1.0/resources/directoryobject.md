---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.
localization_priority: Priority
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4e690598a9e93dbbbc7527bbfcd8864e0b800bc5
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225104"
---
# <a name="directoryobject-resource-type"></a><span data-ttu-id="903dc-104">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="903dc-104">directoryObject resource type</span></span>

<span data-ttu-id="903dc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="903dc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="903dc-p102">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.</span><span class="sxs-lookup"><span data-stu-id="903dc-p102">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="903dc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="903dc-108">Methods</span></span>

| <span data-ttu-id="903dc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="903dc-109">Method</span></span>       | <span data-ttu-id="903dc-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="903dc-110">Return Type</span></span>  |<span data-ttu-id="903dc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="903dc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="903dc-112">Получение объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="903dc-112">Get directoryObject</span></span>](../api/directoryobject-get.md) | [<span data-ttu-id="903dc-113">directoryObject</span><span class="sxs-lookup"><span data-stu-id="903dc-113">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="903dc-114">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="903dc-114">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="903dc-115">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="903dc-115">Delete directoryObject</span></span>](../api/directoryobject-delete.md) | <span data-ttu-id="903dc-116">Нет</span><span class="sxs-lookup"><span data-stu-id="903dc-116">None</span></span> |<span data-ttu-id="903dc-117">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="903dc-117">Delete a directory object.</span></span> |
|[<span data-ttu-id="903dc-118">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="903dc-118">checkMemberGroups</span></span>](../api/directoryobject-checkmembergroups.md)|<span data-ttu-id="903dc-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="903dc-119">String collection</span></span>|<span data-ttu-id="903dc-p103">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="903dc-p103">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="903dc-122">Получение доступных свойств расширения</span><span class="sxs-lookup"><span data-stu-id="903dc-122">Get available extension properties</span></span>](../api/directoryobject-getavailableextensionproperties.md)|<span data-ttu-id="903dc-123">Коллекция [extensionProperty](../resources/extensionproperty.md)</span><span class="sxs-lookup"><span data-stu-id="903dc-123">[extensionProperty](../resources/extensionproperty.md) collection</span></span>|<span data-ttu-id="903dc-124">Получение полного или отфильтрованного списка свойств расширения каталога, которые зарегистрированы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="903dc-124">Get all or a filtered list of the directory extension properties that have been registered in a directory.</span></span>|
|[<span data-ttu-id="903dc-125">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="903dc-125">getMemberGroups</span></span>](../api/directoryobject-getmembergroups.md)|<span data-ttu-id="903dc-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="903dc-126">String collection</span></span>|<span data-ttu-id="903dc-p104">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="903dc-p104">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="903dc-129">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="903dc-129">getMemberObjects</span></span>](../api/directoryobject-getmemberobjects.md)|<span data-ttu-id="903dc-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="903dc-130">String collection</span></span>| <span data-ttu-id="903dc-p105">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="903dc-p105">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="903dc-133">getByIds</span><span class="sxs-lookup"><span data-stu-id="903dc-133">getByIds</span></span>](../api/directoryobject-getbyids.md) | <span data-ttu-id="903dc-134">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="903dc-134">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="903dc-135">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="903dc-135">Get a set of directory objects based on a set of supplied ids.</span></span> |
|[<span data-ttu-id="903dc-136">validateProperties</span><span class="sxs-lookup"><span data-stu-id="903dc-136">validateProperties</span></span>](../api/directoryobject-validateproperties.md)|<span data-ttu-id="903dc-137">Json</span><span class="sxs-lookup"><span data-stu-id="903dc-137">Json</span></span>| <span data-ttu-id="903dc-138">Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования.</span><span class="sxs-lookup"><span data-stu-id="903dc-138">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> |

## <a name="properties"></a><span data-ttu-id="903dc-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="903dc-139">Properties</span></span>

| <span data-ttu-id="903dc-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="903dc-140">Property</span></span>   | <span data-ttu-id="903dc-141">Тип</span><span class="sxs-lookup"><span data-stu-id="903dc-141">Type</span></span> |<span data-ttu-id="903dc-142">Описание</span><span class="sxs-lookup"><span data-stu-id="903dc-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="903dc-143">id</span><span class="sxs-lookup"><span data-stu-id="903dc-143">id</span></span>|<span data-ttu-id="903dc-144">String</span><span class="sxs-lookup"><span data-stu-id="903dc-144">String</span></span>|<span data-ttu-id="903dc-p106">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="903dc-p106">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="903dc-149">Связи</span><span class="sxs-lookup"><span data-stu-id="903dc-149">Relationships</span></span>

<span data-ttu-id="903dc-150">Нет</span><span class="sxs-lookup"><span data-stu-id="903dc-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="903dc-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="903dc-151">JSON representation</span></span>

<span data-ttu-id="903dc-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="903dc-152">Here is a JSON representation of the resource</span></span>

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
