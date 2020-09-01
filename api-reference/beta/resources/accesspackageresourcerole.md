---
title: Тип ресурса Акцесспаккажересаурцероле
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bc0a60043c9877b4c48a889f93fa48a852c3780
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319589"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="16e15-103">Тип ресурса Акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="16e15-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="16e15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16e15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16e15-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета Access — это ссылка на роль, определенную в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="16e15-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="16e15-106">Эту ссылку можно использовать после создания пакета Access, чтобы указать роли каждого из ресурсов каталога, к которым должен предоставлять пакет Access, путем [создания области применения роли ресурса пакета Access](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span><span class="sxs-lookup"><span data-stu-id="16e15-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="16e15-107">Методы</span><span class="sxs-lookup"><span data-stu-id="16e15-107">Methods</span></span>

| <span data-ttu-id="16e15-108">Метод</span><span class="sxs-lookup"><span data-stu-id="16e15-108">Method</span></span>       | <span data-ttu-id="16e15-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="16e15-109">Return Type</span></span> | <span data-ttu-id="16e15-110">Описание</span><span class="sxs-lookup"><span data-stu-id="16e15-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="16e15-111">Список ролей ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="16e15-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="16e15-112">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="16e15-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="16e15-113">Получение списка объектов Акцесспаккажересаурцероле для каталога.</span><span class="sxs-lookup"><span data-stu-id="16e15-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="16e15-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="16e15-114">Properties</span></span>

| <span data-ttu-id="16e15-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="16e15-115">Property</span></span>     | <span data-ttu-id="16e15-116">Тип</span><span class="sxs-lookup"><span data-stu-id="16e15-116">Type</span></span>        | <span data-ttu-id="16e15-117">Описание</span><span class="sxs-lookup"><span data-stu-id="16e15-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16e15-118">description</span><span class="sxs-lookup"><span data-stu-id="16e15-118">description</span></span>|<span data-ttu-id="16e15-119">String</span><span class="sxs-lookup"><span data-stu-id="16e15-119">String</span></span>|<span data-ttu-id="16e15-120">Описание роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="16e15-120">A description for the resource role.</span></span>|
|<span data-ttu-id="16e15-121">displayName</span><span class="sxs-lookup"><span data-stu-id="16e15-121">displayName</span></span>|<span data-ttu-id="16e15-122">String</span><span class="sxs-lookup"><span data-stu-id="16e15-122">String</span></span>|<span data-ttu-id="16e15-123">Отображаемое имя роли ресурса, например роль, определяемую приложением.</span><span class="sxs-lookup"><span data-stu-id="16e15-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="16e15-124">id</span><span class="sxs-lookup"><span data-stu-id="16e15-124">id</span></span>|<span data-ttu-id="16e15-125">String</span><span class="sxs-lookup"><span data-stu-id="16e15-125">String</span></span>| <span data-ttu-id="16e15-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16e15-126">Read-only.</span></span>|
|<span data-ttu-id="16e15-127">оригинид</span><span class="sxs-lookup"><span data-stu-id="16e15-127">originId</span></span>|<span data-ttu-id="16e15-128">String</span><span class="sxs-lookup"><span data-stu-id="16e15-128">String</span></span>|<span data-ttu-id="16e15-129">Уникальный идентификатор роли ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="16e15-129">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="16e15-130">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="16e15-130">originSystem</span></span>|<span data-ttu-id="16e15-131">String</span><span class="sxs-lookup"><span data-stu-id="16e15-131">String</span></span>|<span data-ttu-id="16e15-132">Тип ресурса в исходной системе, например `SharePointOnline` , `AadApplication` или `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="16e15-132">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16e15-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="16e15-133">Relationships</span></span>

| <span data-ttu-id="16e15-134">Связь</span><span class="sxs-lookup"><span data-stu-id="16e15-134">Relationship</span></span> | <span data-ttu-id="16e15-135">Тип</span><span class="sxs-lookup"><span data-stu-id="16e15-135">Type</span></span>        | <span data-ttu-id="16e15-136">Описание</span><span class="sxs-lookup"><span data-stu-id="16e15-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16e15-137">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="16e15-137">accessPackageResource</span></span>|[<span data-ttu-id="16e15-138">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="16e15-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="16e15-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="16e15-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16e15-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16e15-141">JSON representation</span></span>

<span data-ttu-id="16e15-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16e15-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "baseType": "",
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
