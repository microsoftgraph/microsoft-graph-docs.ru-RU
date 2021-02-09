---
title: Тип ресурса accessPackageResourceRole
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 188504dc96628ba0047f9feb2489e94b8f138874
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158578"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="1e9a5-103">Тип ресурса accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="1e9a5-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="1e9a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e9a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e9a5-105">В [управлении правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета доступа является ссылкой на роль, определенную в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="1e9a5-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="1e9a5-106">Эта ссылка может использоваться после создания пакета доступа для указания ролей каждого из ресурсов каталога, в которые должен доставляться пакет доступа, путем создания области роли ресурса пакета [доступа.](../api/accesspackage-post-accesspackageresourcerolescopes.md)</span><span class="sxs-lookup"><span data-stu-id="1e9a5-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1e9a5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1e9a5-107">Methods</span></span>

| <span data-ttu-id="1e9a5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1e9a5-108">Method</span></span>       | <span data-ttu-id="1e9a5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e9a5-109">Return Type</span></span> | <span data-ttu-id="1e9a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1e9a5-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1e9a5-111">Список ролей ресурсов accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="1e9a5-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="1e9a5-112">[Коллекция accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="1e9a5-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="1e9a5-113">Получить список объектов accessPackageResourceRole для каталога.</span><span class="sxs-lookup"><span data-stu-id="1e9a5-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e9a5-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e9a5-114">Properties</span></span>

| <span data-ttu-id="1e9a5-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e9a5-115">Property</span></span>     | <span data-ttu-id="1e9a5-116">Тип</span><span class="sxs-lookup"><span data-stu-id="1e9a5-116">Type</span></span>        | <span data-ttu-id="1e9a5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1e9a5-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e9a5-118">description</span><span class="sxs-lookup"><span data-stu-id="1e9a5-118">description</span></span>|<span data-ttu-id="1e9a5-119">String</span><span class="sxs-lookup"><span data-stu-id="1e9a5-119">String</span></span>|<span data-ttu-id="1e9a5-120">Описание роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="1e9a5-120">A description for the resource role.</span></span>|
|<span data-ttu-id="1e9a5-121">displayName</span><span class="sxs-lookup"><span data-stu-id="1e9a5-121">displayName</span></span>|<span data-ttu-id="1e9a5-122">String</span><span class="sxs-lookup"><span data-stu-id="1e9a5-122">String</span></span>|<span data-ttu-id="1e9a5-123">Отображаемого имени роли ресурса, например роли, определенной приложением.</span><span class="sxs-lookup"><span data-stu-id="1e9a5-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="1e9a5-124">id</span><span class="sxs-lookup"><span data-stu-id="1e9a5-124">id</span></span>|<span data-ttu-id="1e9a5-125">String</span><span class="sxs-lookup"><span data-stu-id="1e9a5-125">String</span></span>| <span data-ttu-id="1e9a5-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1e9a5-126">Read-only.</span></span>|
|<span data-ttu-id="1e9a5-127">originId</span><span class="sxs-lookup"><span data-stu-id="1e9a5-127">originId</span></span>|<span data-ttu-id="1e9a5-128">String</span><span class="sxs-lookup"><span data-stu-id="1e9a5-128">String</span></span>|<span data-ttu-id="1e9a5-129">Уникальный идентификатор роли ресурса в системе источника.</span><span class="sxs-lookup"><span data-stu-id="1e9a5-129">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="1e9a5-130">originSystem</span><span class="sxs-lookup"><span data-stu-id="1e9a5-130">originSystem</span></span>|<span data-ttu-id="1e9a5-131">String</span><span class="sxs-lookup"><span data-stu-id="1e9a5-131">String</span></span>|<span data-ttu-id="1e9a5-132">Тип ресурса в системе источника, например `SharePointOnline` , или `AadApplication` `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="1e9a5-132">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e9a5-133">Связи</span><span class="sxs-lookup"><span data-stu-id="1e9a5-133">Relationships</span></span>

| <span data-ttu-id="1e9a5-134">Связь</span><span class="sxs-lookup"><span data-stu-id="1e9a5-134">Relationship</span></span> | <span data-ttu-id="1e9a5-135">Тип</span><span class="sxs-lookup"><span data-stu-id="1e9a5-135">Type</span></span>        | <span data-ttu-id="1e9a5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="1e9a5-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e9a5-137">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="1e9a5-137">accessPackageResource</span></span>|[<span data-ttu-id="1e9a5-138">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="1e9a5-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="1e9a5-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1e9a5-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e9a5-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e9a5-141">JSON representation</span></span>

<span data-ttu-id="1e9a5-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e9a5-142">The following is a JSON representation of the resource.</span></span>

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


