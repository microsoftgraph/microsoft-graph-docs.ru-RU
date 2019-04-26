---
title: Тип ресурса Говернанцероледефинитион
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.
localization_priority: Normal
ms.openlocfilehash: 27b4b144f834f3b5eb4270a2875da5add10efb9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333759"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="24574-104">Тип ресурса Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="24574-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="24574-105">Представляет определения ролей.</span><span class="sxs-lookup"><span data-stu-id="24574-105">Represents the role definitions.</span></span> <span data-ttu-id="24574-106">Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.</span><span class="sxs-lookup"><span data-stu-id="24574-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="24574-107">Методы</span><span class="sxs-lookup"><span data-stu-id="24574-107">Methods</span></span>

| <span data-ttu-id="24574-108">Метод</span><span class="sxs-lookup"><span data-stu-id="24574-108">Method</span></span>          | <span data-ttu-id="24574-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="24574-109">Return Type</span></span> |<span data-ttu-id="24574-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24574-110">Description</span></span>|
|:---------------|:--------|:--------|:----------|
|[<span data-ttu-id="24574-111">Список</span><span class="sxs-lookup"><span data-stu-id="24574-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="24574-112">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24574-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="24574-113">ПереЧисление коллекции определений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="24574-113">List a collection of role definitions on a resource.</span></span>|
|[<span data-ttu-id="24574-114">Получение</span><span class="sxs-lookup"><span data-stu-id="24574-114">Get</span></span>](../api/governanceroledefinition-get.md) | [<span data-ttu-id="24574-115">Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="24574-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="24574-116">Считывание свойств и связей объекта определения роли, указанного по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="24574-116">Read properties and relationships of a role definition entity specified by id.</span></span>|
<span data-ttu-id="24574-117">Нет `POST`, `PUT`, `PATCH`, `DELETE` поддерживается в `roleDefinitions` наборе сущностей для Now.</span><span class="sxs-lookup"><span data-stu-id="24574-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>
## <a name="properties"></a><span data-ttu-id="24574-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="24574-118">Properties</span></span>
| <span data-ttu-id="24574-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="24574-119">Property</span></span>  | <span data-ttu-id="24574-120">Тип</span><span class="sxs-lookup"><span data-stu-id="24574-120">Type</span></span>      |<span data-ttu-id="24574-121">Описание</span><span class="sxs-lookup"><span data-stu-id="24574-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="24574-122">id</span><span class="sxs-lookup"><span data-stu-id="24574-122">id</span></span>         |<span data-ttu-id="24574-123">Строка</span><span class="sxs-lookup"><span data-stu-id="24574-123">String</span></span>     |<span data-ttu-id="24574-124">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="24574-124">The id of the role definition.</span></span> |
|<span data-ttu-id="24574-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="24574-125">resourceId</span></span> |<span data-ttu-id="24574-126">String</span><span class="sxs-lookup"><span data-stu-id="24574-126">String</span></span>     |<span data-ttu-id="24574-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24574-127">Required.</span></span> <span data-ttu-id="24574-128">Идентификатор ресурса, связанного с определением роли.</span><span class="sxs-lookup"><span data-stu-id="24574-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="24574-129">externalId</span><span class="sxs-lookup"><span data-stu-id="24574-129">externalId</span></span>   |<span data-ttu-id="24574-130">String</span><span class="sxs-lookup"><span data-stu-id="24574-130">String</span></span>     |<span data-ttu-id="24574-131">Внешний идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="24574-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="24574-132">displayName</span><span class="sxs-lookup"><span data-stu-id="24574-132">displayName</span></span>|<span data-ttu-id="24574-133">Строка</span><span class="sxs-lookup"><span data-stu-id="24574-133">String</span></span>     |<span data-ttu-id="24574-134">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="24574-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="24574-135">templateId</span><span class="sxs-lookup"><span data-stu-id="24574-135">templateId</span></span> | <span data-ttu-id="24574-136">String</span><span class="sxs-lookup"><span data-stu-id="24574-136">String</span></span> | |

## <a name="relationships"></a><span data-ttu-id="24574-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="24574-137">Relationships</span></span>
| <span data-ttu-id="24574-138">Отношение</span><span class="sxs-lookup"><span data-stu-id="24574-138">Relationship</span></span> | <span data-ttu-id="24574-139">Тип</span><span class="sxs-lookup"><span data-stu-id="24574-139">Type</span></span>   |<span data-ttu-id="24574-140">Описание</span><span class="sxs-lookup"><span data-stu-id="24574-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24574-141">resource</span><span class="sxs-lookup"><span data-stu-id="24574-141">resource</span></span>|[<span data-ttu-id="24574-142">governanceResource</span><span class="sxs-lookup"><span data-stu-id="24574-142">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="24574-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24574-143">Read-only.</span></span> <span data-ttu-id="24574-144">Связанный ресурс для определения роли.</span><span class="sxs-lookup"><span data-stu-id="24574-144">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="24574-145">Ролесеттинг</span><span class="sxs-lookup"><span data-stu-id="24574-145">roleSetting</span></span>|[<span data-ttu-id="24574-146">Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="24574-146">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="24574-147">Связанный параметр роли для определения роли.</span><span class="sxs-lookup"><span data-stu-id="24574-147">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24574-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24574-148">JSON representation</span></span>

<span data-ttu-id="24574-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24574-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",  
  "templateId":"String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
