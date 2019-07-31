---
title: Тип ресурса Говернанцероледефинитион
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 668f5430e8f098986b7d5398f32c9c35543a7e11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971855"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="4ecb6-104">Тип ресурса Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="4ecb6-104">governanceRoleDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="4ecb6-105">Представляет определения ролей.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-105">Represents the role definitions.</span></span> <span data-ttu-id="4ecb6-106">Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-106">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="4ecb6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4ecb6-107">Methods</span></span>

| <span data-ttu-id="4ecb6-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4ecb6-108">Method</span></span>          | <span data-ttu-id="4ecb6-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ecb6-109">Return Type</span></span> |<span data-ttu-id="4ecb6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ecb6-110">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="4ecb6-111">List</span><span class="sxs-lookup"><span data-stu-id="4ecb6-111">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="4ecb6-112">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4ecb6-112">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="4ecb6-113">Перечисление коллекции определений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-113">List a collection of role definitions on a resource.</span></span>|
|<span data-ttu-id="4ecb6-114">[получение](../api/governanceroledefinition-get.md);</span><span class="sxs-lookup"><span data-stu-id="4ecb6-114">[Get](../api/governanceroledefinition-get.md)</span></span> | [<span data-ttu-id="4ecb6-115">Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="4ecb6-115">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="4ecb6-116">Считывание свойств и связей объекта определения роли, указанного по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-116">Read properties and relationships of a role definition entity specified by id.</span></span>|

<span data-ttu-id="4ecb6-117">Нет `POST`, `PUT`, `PATCH`, `DELETE` поддерживается в `roleDefinitions` наборе сущностей для Now.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-117">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="4ecb6-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ecb6-118">Properties</span></span>
| <span data-ttu-id="4ecb6-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ecb6-119">Property</span></span>  | <span data-ttu-id="4ecb6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4ecb6-120">Type</span></span>      |<span data-ttu-id="4ecb6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4ecb6-121">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="4ecb6-122">id</span><span class="sxs-lookup"><span data-stu-id="4ecb6-122">id</span></span>         |<span data-ttu-id="4ecb6-123">Строка</span><span class="sxs-lookup"><span data-stu-id="4ecb6-123">String</span></span>     |<span data-ttu-id="4ecb6-124">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-124">The id of the role definition.</span></span> |
|<span data-ttu-id="4ecb6-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="4ecb6-125">resourceId</span></span> |<span data-ttu-id="4ecb6-126">String</span><span class="sxs-lookup"><span data-stu-id="4ecb6-126">String</span></span>     |<span data-ttu-id="4ecb6-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-127">Required.</span></span> <span data-ttu-id="4ecb6-128">Идентификатор ресурса, связанного с определением роли.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-128">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="4ecb6-129">externalId</span><span class="sxs-lookup"><span data-stu-id="4ecb6-129">externalId</span></span>   |<span data-ttu-id="4ecb6-130">String</span><span class="sxs-lookup"><span data-stu-id="4ecb6-130">String</span></span>     |<span data-ttu-id="4ecb6-131">Внешний идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-131">The external id of the role definition.</span></span>|
|<span data-ttu-id="4ecb6-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4ecb6-132">displayName</span></span>|<span data-ttu-id="4ecb6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4ecb6-133">String</span></span>     |<span data-ttu-id="4ecb6-134">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-134">The display name of the role definition.</span></span>|
|<span data-ttu-id="4ecb6-135">templateId</span><span class="sxs-lookup"><span data-stu-id="4ecb6-135">templateId</span></span> | <span data-ttu-id="4ecb6-136">String</span><span class="sxs-lookup"><span data-stu-id="4ecb6-136">String</span></span> | |

## <a name="relationships"></a><span data-ttu-id="4ecb6-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="4ecb6-137">Relationships</span></span>
| <span data-ttu-id="4ecb6-138">Отношение</span><span class="sxs-lookup"><span data-stu-id="4ecb6-138">Relationship</span></span> | <span data-ttu-id="4ecb6-139">Тип</span><span class="sxs-lookup"><span data-stu-id="4ecb6-139">Type</span></span>   |<span data-ttu-id="4ecb6-140">Описание</span><span class="sxs-lookup"><span data-stu-id="4ecb6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ecb6-141">resource</span><span class="sxs-lookup"><span data-stu-id="4ecb6-141">resource</span></span>|[<span data-ttu-id="4ecb6-142">governanceResource</span><span class="sxs-lookup"><span data-stu-id="4ecb6-142">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="4ecb6-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-143">Read-only.</span></span> <span data-ttu-id="4ecb6-144">Связанный ресурс для определения роли.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-144">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="4ecb6-145">Ролесеттинг</span><span class="sxs-lookup"><span data-stu-id="4ecb6-145">roleSetting</span></span>|[<span data-ttu-id="4ecb6-146">Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="4ecb6-146">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="4ecb6-147">Связанный параметр роли для определения роли.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-147">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ecb6-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ecb6-148">JSON representation</span></span>

<span data-ttu-id="4ecb6-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ecb6-149">Here is a JSON representation of the resource.</span></span>

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
