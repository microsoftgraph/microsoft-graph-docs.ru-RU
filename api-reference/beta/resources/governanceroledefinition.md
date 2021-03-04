---
title: тип ресурса governanceRoleDefinition
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, Contributor и т.д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: dd4a9fc90d3c12669464a5e9b931b968d4526640
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443057"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="897de-104">тип ресурса governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="897de-104">governanceRoleDefinition resource type</span></span>

<span data-ttu-id="897de-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="897de-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="897de-106">Представляет определения ролей.</span><span class="sxs-lookup"><span data-stu-id="897de-106">Represents the role definitions.</span></span> <span data-ttu-id="897de-107">Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, Contributor и т.д.</span><span class="sxs-lookup"><span data-stu-id="897de-107">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="897de-108">Методы</span><span class="sxs-lookup"><span data-stu-id="897de-108">Methods</span></span>

| <span data-ttu-id="897de-109">Метод</span><span class="sxs-lookup"><span data-stu-id="897de-109">Method</span></span>          | <span data-ttu-id="897de-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="897de-110">Return Type</span></span> |<span data-ttu-id="897de-111">Описание</span><span class="sxs-lookup"><span data-stu-id="897de-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="897de-112">Список</span><span class="sxs-lookup"><span data-stu-id="897de-112">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="897de-113">[коллекция governanceRoleDefinition](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="897de-113">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="897de-114">Список коллекции определений ролей на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="897de-114">List a collection of role definitions on a resource.</span></span>|
|<span data-ttu-id="897de-115">[получение](../api/governanceroledefinition-get.md);</span><span class="sxs-lookup"><span data-stu-id="897de-115">[Get](../api/governanceroledefinition-get.md)</span></span> | [<span data-ttu-id="897de-116">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="897de-116">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="897de-117">Чтение свойств и связей сущности определения роли, указанной в id.</span><span class="sxs-lookup"><span data-stu-id="897de-117">Read properties and relationships of a role definition entity specified by id.</span></span>|

<span data-ttu-id="897de-118">`POST`Нет, `PUT` `PATCH` `DELETE` поддерживается в `roleDefinitions` наборе сущности на данный момент.</span><span class="sxs-lookup"><span data-stu-id="897de-118">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="897de-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="897de-119">Properties</span></span>
| <span data-ttu-id="897de-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="897de-120">Property</span></span>    | <span data-ttu-id="897de-121">Тип</span><span class="sxs-lookup"><span data-stu-id="897de-121">Type</span></span>   | <span data-ttu-id="897de-122">Описание</span><span class="sxs-lookup"><span data-stu-id="897de-122">Description</span></span>                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| <span data-ttu-id="897de-123">id</span><span class="sxs-lookup"><span data-stu-id="897de-123">id</span></span>          | <span data-ttu-id="897de-124">String</span><span class="sxs-lookup"><span data-stu-id="897de-124">String</span></span> | <span data-ttu-id="897de-125">ID определения роли.</span><span class="sxs-lookup"><span data-stu-id="897de-125">The id of the role definition.</span></span>                                        |
| <span data-ttu-id="897de-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="897de-126">resourceId</span></span>  | <span data-ttu-id="897de-127">String</span><span class="sxs-lookup"><span data-stu-id="897de-127">String</span></span> | <span data-ttu-id="897de-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="897de-128">Required.</span></span> <span data-ttu-id="897de-129">ID ресурса, связанного с определением роли.</span><span class="sxs-lookup"><span data-stu-id="897de-129">The id of the resource associated with the role definition.</span></span> |
| <span data-ttu-id="897de-130">externalId</span><span class="sxs-lookup"><span data-stu-id="897de-130">externalId</span></span>  | <span data-ttu-id="897de-131">String</span><span class="sxs-lookup"><span data-stu-id="897de-131">String</span></span> | <span data-ttu-id="897de-132">Внешний id определения роли.</span><span class="sxs-lookup"><span data-stu-id="897de-132">The external id of the role definition.</span></span>                               |
| <span data-ttu-id="897de-133">displayName</span><span class="sxs-lookup"><span data-stu-id="897de-133">displayName</span></span> | <span data-ttu-id="897de-134">String</span><span class="sxs-lookup"><span data-stu-id="897de-134">String</span></span> | <span data-ttu-id="897de-135">Отображение имени определения роли.</span><span class="sxs-lookup"><span data-stu-id="897de-135">The display name of the role definition.</span></span>                              |
| <span data-ttu-id="897de-136">templateId</span><span class="sxs-lookup"><span data-stu-id="897de-136">templateId</span></span>  | <span data-ttu-id="897de-137">String</span><span class="sxs-lookup"><span data-stu-id="897de-137">String</span></span> |                                                                       |

## <a name="relationships"></a><span data-ttu-id="897de-138">Связи</span><span class="sxs-lookup"><span data-stu-id="897de-138">Relationships</span></span>
| <span data-ttu-id="897de-139">Связь</span><span class="sxs-lookup"><span data-stu-id="897de-139">Relationship</span></span> | <span data-ttu-id="897de-140">Тип</span><span class="sxs-lookup"><span data-stu-id="897de-140">Type</span></span>   |<span data-ttu-id="897de-141">Описание</span><span class="sxs-lookup"><span data-stu-id="897de-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="897de-142">resource</span><span class="sxs-lookup"><span data-stu-id="897de-142">resource</span></span>|[<span data-ttu-id="897de-143">governanceResource</span><span class="sxs-lookup"><span data-stu-id="897de-143">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="897de-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="897de-144">Read-only.</span></span> <span data-ttu-id="897de-145">Связанный ресурс для определения роли.</span><span class="sxs-lookup"><span data-stu-id="897de-145">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="897de-146">roleSetting</span><span class="sxs-lookup"><span data-stu-id="897de-146">roleSetting</span></span>|[<span data-ttu-id="897de-147">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="897de-147">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="897de-148">Связанный параметр роли для определения роли.</span><span class="sxs-lookup"><span data-stu-id="897de-148">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="897de-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="897de-149">JSON representation</span></span>

<span data-ttu-id="897de-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="897de-150">Here is a JSON representation of the resource.</span></span>

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


