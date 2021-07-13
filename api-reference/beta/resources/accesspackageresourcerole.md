---
title: тип ресурса accessPackageResourceRole
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1194c27e929a14f738384441ab57f5090d8b1149
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401609"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="5dd7b-103">тип ресурса accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="5dd7b-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="5dd7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dd7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dd7b-105">В [управлении правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета доступа является ссылкой на роль, определенную в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="5dd7b-106">Эта ссылка может быть использована после создания пакета доступа для указания ролей каждого из ресурсов каталога, в которые должен доставить пакет доступа, путем создания области ролей ресурсов пакета [доступа.](../api/accesspackage-post-accesspackageresourcerolescopes.md)</span><span class="sxs-lookup"><span data-stu-id="5dd7b-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5dd7b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5dd7b-107">Methods</span></span>

| <span data-ttu-id="5dd7b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5dd7b-108">Method</span></span>       | <span data-ttu-id="5dd7b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5dd7b-109">Return Type</span></span> | <span data-ttu-id="5dd7b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5dd7b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5dd7b-111">Роли ресурсов accessPackageCatalog в списке</span><span class="sxs-lookup"><span data-stu-id="5dd7b-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="5dd7b-112">[коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="5dd7b-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="5dd7b-113">Извлечение списка объектов accessPackageResourceRole для каталога.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="5dd7b-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dd7b-114">Properties</span></span>

| <span data-ttu-id="5dd7b-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dd7b-115">Property</span></span>     | <span data-ttu-id="5dd7b-116">Тип</span><span class="sxs-lookup"><span data-stu-id="5dd7b-116">Type</span></span>        | <span data-ttu-id="5dd7b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5dd7b-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5dd7b-118">description</span><span class="sxs-lookup"><span data-stu-id="5dd7b-118">description</span></span>|<span data-ttu-id="5dd7b-119">String</span><span class="sxs-lookup"><span data-stu-id="5dd7b-119">String</span></span>|<span data-ttu-id="5dd7b-120">Описание роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-120">A description for the resource role.</span></span>|
|<span data-ttu-id="5dd7b-121">displayName</span><span class="sxs-lookup"><span data-stu-id="5dd7b-121">displayName</span></span>|<span data-ttu-id="5dd7b-122">String</span><span class="sxs-lookup"><span data-stu-id="5dd7b-122">String</span></span>|<span data-ttu-id="5dd7b-123">Отображение имени роли ресурса, например роли, определенной приложением.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="5dd7b-124">id</span><span class="sxs-lookup"><span data-stu-id="5dd7b-124">id</span></span>|<span data-ttu-id="5dd7b-125">String</span><span class="sxs-lookup"><span data-stu-id="5dd7b-125">String</span></span>| <span data-ttu-id="5dd7b-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-126">Read-only.</span></span>|
|<span data-ttu-id="5dd7b-127">OriginId</span><span class="sxs-lookup"><span data-stu-id="5dd7b-127">originId</span></span>|<span data-ttu-id="5dd7b-128">String</span><span class="sxs-lookup"><span data-stu-id="5dd7b-128">String</span></span>|<span data-ttu-id="5dd7b-129">Уникальный идентификатор роли ресурса в системе происхождения.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-129">The unique identifier of the resource role in the origin system.</span></span> <span data-ttu-id="5dd7b-130">Для сайта SharePoint Online originId будет номером последовательности роли на сайте.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-130">For a SharePoint Online site, the originId will be the sequence number of the role in the site.</span></span> |
|<span data-ttu-id="5dd7b-131">originSystem</span><span class="sxs-lookup"><span data-stu-id="5dd7b-131">originSystem</span></span>|<span data-ttu-id="5dd7b-132">String</span><span class="sxs-lookup"><span data-stu-id="5dd7b-132">String</span></span>|<span data-ttu-id="5dd7b-133">Тип ресурса в системе происхождения, например `SharePointOnline` , `AadApplication` или `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="5dd7b-133">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dd7b-134">Связи</span><span class="sxs-lookup"><span data-stu-id="5dd7b-134">Relationships</span></span>

| <span data-ttu-id="5dd7b-135">Связь</span><span class="sxs-lookup"><span data-stu-id="5dd7b-135">Relationship</span></span> | <span data-ttu-id="5dd7b-136">Тип</span><span class="sxs-lookup"><span data-stu-id="5dd7b-136">Type</span></span>        | <span data-ttu-id="5dd7b-137">Описание</span><span class="sxs-lookup"><span data-stu-id="5dd7b-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5dd7b-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="5dd7b-138">accessPackageResource</span></span>|[<span data-ttu-id="5dd7b-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="5dd7b-139">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="5dd7b-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dd7b-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5dd7b-142">JSON representation</span></span>

<span data-ttu-id="5dd7b-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dd7b-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


