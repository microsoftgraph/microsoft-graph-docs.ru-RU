---
title: Тип ресурса Говернанцероледефинитион
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 985e674c0e8e79f7b929097dd5c61dfa15917a93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497393"
---
# <a name="governanceroledefinition-resource-type"></a><span data-ttu-id="ed181-104">Тип ресурса Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="ed181-104">governanceRoleDefinition resource type</span></span>

<span data-ttu-id="ed181-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ed181-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="ed181-106">Представляет определения ролей.</span><span class="sxs-lookup"><span data-stu-id="ed181-106">Represents the role definitions.</span></span> <span data-ttu-id="ed181-107">Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.</span><span class="sxs-lookup"><span data-stu-id="ed181-107">For Azure resources, it can represent Azure RBAC roles, such as Owner, Reader, Contributor, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="ed181-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ed181-108">Methods</span></span>

| <span data-ttu-id="ed181-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ed181-109">Method</span></span>          | <span data-ttu-id="ed181-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed181-110">Return Type</span></span> |<span data-ttu-id="ed181-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed181-111">Description</span></span>|
|:---------------|:--------|:--------|
|[<span data-ttu-id="ed181-112">List</span><span class="sxs-lookup"><span data-stu-id="ed181-112">List</span></span>](../api/governanceroledefinition-list.md) | <span data-ttu-id="ed181-113">Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ed181-113">[governanceRoleDefinition](../resources/governanceroledefinition.md) collection</span></span> |<span data-ttu-id="ed181-114">Перечисление коллекции определений ролей для ресурса.</span><span class="sxs-lookup"><span data-stu-id="ed181-114">List a collection of role definitions on a resource.</span></span>|
|<span data-ttu-id="ed181-115">[получение](../api/governanceroledefinition-get.md);</span><span class="sxs-lookup"><span data-stu-id="ed181-115">[Get](../api/governanceroledefinition-get.md)</span></span> | [<span data-ttu-id="ed181-116">governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ed181-116">governanceRoleDefinition</span></span>](../resources/governanceroledefinition.md) |<span data-ttu-id="ed181-117">Считывание свойств и связей объекта определения роли, указанного по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="ed181-117">Read properties and relationships of a role definition entity specified by id.</span></span>|

<span data-ttu-id="ed181-118">Нет `POST`, `PUT`, `PATCH`, `DELETE` поддерживается в `roleDefinitions` наборе сущностей для Now.</span><span class="sxs-lookup"><span data-stu-id="ed181-118">No `POST`, `PUT`, `PATCH`, `DELETE` is supported on `roleDefinitions` entity set for now.</span></span>

## <a name="properties"></a><span data-ttu-id="ed181-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed181-119">Properties</span></span>
| <span data-ttu-id="ed181-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed181-120">Property</span></span>  | <span data-ttu-id="ed181-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ed181-121">Type</span></span>      |<span data-ttu-id="ed181-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ed181-122">Description</span></span>|
|:----|:----------|:----------|:----------|
|<span data-ttu-id="ed181-123">id</span><span class="sxs-lookup"><span data-stu-id="ed181-123">id</span></span>         |<span data-ttu-id="ed181-124">Строка</span><span class="sxs-lookup"><span data-stu-id="ed181-124">String</span></span>     |<span data-ttu-id="ed181-125">Идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="ed181-125">The id of the role definition.</span></span> |
|<span data-ttu-id="ed181-126">resourceId</span><span class="sxs-lookup"><span data-stu-id="ed181-126">resourceId</span></span> |<span data-ttu-id="ed181-127">String</span><span class="sxs-lookup"><span data-stu-id="ed181-127">String</span></span>     |<span data-ttu-id="ed181-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed181-128">Required.</span></span> <span data-ttu-id="ed181-129">Идентификатор ресурса, связанного с определением роли.</span><span class="sxs-lookup"><span data-stu-id="ed181-129">The id of the resource associated with the role definition.</span></span> |
|<span data-ttu-id="ed181-130">externalId</span><span class="sxs-lookup"><span data-stu-id="ed181-130">externalId</span></span>   |<span data-ttu-id="ed181-131">String</span><span class="sxs-lookup"><span data-stu-id="ed181-131">String</span></span>     |<span data-ttu-id="ed181-132">Внешний идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="ed181-132">The external id of the role definition.</span></span>|
|<span data-ttu-id="ed181-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ed181-133">displayName</span></span>|<span data-ttu-id="ed181-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ed181-134">String</span></span>     |<span data-ttu-id="ed181-135">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="ed181-135">The display name of the role definition.</span></span>|
|<span data-ttu-id="ed181-136">templateId</span><span class="sxs-lookup"><span data-stu-id="ed181-136">templateId</span></span> | <span data-ttu-id="ed181-137">String</span><span class="sxs-lookup"><span data-stu-id="ed181-137">String</span></span> | |

## <a name="relationships"></a><span data-ttu-id="ed181-138">Связи</span><span class="sxs-lookup"><span data-stu-id="ed181-138">Relationships</span></span>
| <span data-ttu-id="ed181-139">Связь</span><span class="sxs-lookup"><span data-stu-id="ed181-139">Relationship</span></span> | <span data-ttu-id="ed181-140">Тип</span><span class="sxs-lookup"><span data-stu-id="ed181-140">Type</span></span>   |<span data-ttu-id="ed181-141">Описание</span><span class="sxs-lookup"><span data-stu-id="ed181-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed181-142">resource</span><span class="sxs-lookup"><span data-stu-id="ed181-142">resource</span></span>|[<span data-ttu-id="ed181-143">governanceResource</span><span class="sxs-lookup"><span data-stu-id="ed181-143">governanceResource</span></span>](../resources/governanceresource.md)|<span data-ttu-id="ed181-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed181-144">Read-only.</span></span> <span data-ttu-id="ed181-145">Связанный ресурс для определения роли.</span><span class="sxs-lookup"><span data-stu-id="ed181-145">The associated resource for the role definition.</span></span>|
|<span data-ttu-id="ed181-146">ролесеттинг</span><span class="sxs-lookup"><span data-stu-id="ed181-146">roleSetting</span></span>|[<span data-ttu-id="ed181-147">governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="ed181-147">governanceRoleSetting</span></span>](../resources/governancerolesetting.md)|<span data-ttu-id="ed181-148">Связанный параметр роли для определения роли.</span><span class="sxs-lookup"><span data-stu-id="ed181-148">The associated role setting for the role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed181-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed181-149">JSON representation</span></span>

<span data-ttu-id="ed181-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed181-150">Here is a JSON representation of the resource.</span></span>

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
