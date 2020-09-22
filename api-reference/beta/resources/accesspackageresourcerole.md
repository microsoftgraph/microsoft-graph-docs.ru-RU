---
title: Тип ресурса Акцесспаккажересаурцероле
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff36109d59ee0bef4d81caf16c16f69f26b0a03e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042809"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="331f1-103">Тип ресурса Акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="331f1-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="331f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="331f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="331f1-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета Access — это ссылка на роль, определенную в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="331f1-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource.</span></span> <span data-ttu-id="331f1-106">Эту ссылку можно использовать после создания пакета Access, чтобы указать роли каждого из ресурсов каталога, к которым должен предоставлять пакет Access, путем [создания области применения роли ресурса пакета Access](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span><span class="sxs-lookup"><span data-stu-id="331f1-106">That reference can be used after creating an access package to specify the roles of each of the catalog's resources into which an access package should deliver, by [creating an access package resource role scope](../api/accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="methods"></a><span data-ttu-id="331f1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="331f1-107">Methods</span></span>

| <span data-ttu-id="331f1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="331f1-108">Method</span></span>       | <span data-ttu-id="331f1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="331f1-109">Return Type</span></span> | <span data-ttu-id="331f1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="331f1-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="331f1-111">Список ролей ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="331f1-111">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="331f1-112">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="331f1-112">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="331f1-113">Получение списка объектов Акцесспаккажересаурцероле для каталога.</span><span class="sxs-lookup"><span data-stu-id="331f1-113">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="331f1-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="331f1-114">Properties</span></span>

| <span data-ttu-id="331f1-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="331f1-115">Property</span></span>     | <span data-ttu-id="331f1-116">Тип</span><span class="sxs-lookup"><span data-stu-id="331f1-116">Type</span></span>        | <span data-ttu-id="331f1-117">Описание</span><span class="sxs-lookup"><span data-stu-id="331f1-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="331f1-118">description</span><span class="sxs-lookup"><span data-stu-id="331f1-118">description</span></span>|<span data-ttu-id="331f1-119">String</span><span class="sxs-lookup"><span data-stu-id="331f1-119">String</span></span>|<span data-ttu-id="331f1-120">Описание роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="331f1-120">A description for the resource role.</span></span>|
|<span data-ttu-id="331f1-121">displayName</span><span class="sxs-lookup"><span data-stu-id="331f1-121">displayName</span></span>|<span data-ttu-id="331f1-122">Строка</span><span class="sxs-lookup"><span data-stu-id="331f1-122">String</span></span>|<span data-ttu-id="331f1-123">Отображаемое имя роли ресурса, например роль, определяемую приложением.</span><span class="sxs-lookup"><span data-stu-id="331f1-123">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="331f1-124">id</span><span class="sxs-lookup"><span data-stu-id="331f1-124">id</span></span>|<span data-ttu-id="331f1-125">String</span><span class="sxs-lookup"><span data-stu-id="331f1-125">String</span></span>| <span data-ttu-id="331f1-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="331f1-126">Read-only.</span></span>|
|<span data-ttu-id="331f1-127">оригинид</span><span class="sxs-lookup"><span data-stu-id="331f1-127">originId</span></span>|<span data-ttu-id="331f1-128">Строка</span><span class="sxs-lookup"><span data-stu-id="331f1-128">String</span></span>|<span data-ttu-id="331f1-129">Уникальный идентификатор роли ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="331f1-129">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="331f1-130">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="331f1-130">originSystem</span></span>|<span data-ttu-id="331f1-131">Строка</span><span class="sxs-lookup"><span data-stu-id="331f1-131">String</span></span>|<span data-ttu-id="331f1-132">Тип ресурса в исходной системе, например `SharePointOnline` , `AadApplication` или `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="331f1-132">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="331f1-133">Связи</span><span class="sxs-lookup"><span data-stu-id="331f1-133">Relationships</span></span>

| <span data-ttu-id="331f1-134">Связь</span><span class="sxs-lookup"><span data-stu-id="331f1-134">Relationship</span></span> | <span data-ttu-id="331f1-135">Тип</span><span class="sxs-lookup"><span data-stu-id="331f1-135">Type</span></span>        | <span data-ttu-id="331f1-136">Описание</span><span class="sxs-lookup"><span data-stu-id="331f1-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="331f1-137">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="331f1-137">accessPackageResource</span></span>|[<span data-ttu-id="331f1-138">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="331f1-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="331f1-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="331f1-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="331f1-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="331f1-141">JSON representation</span></span>

<span data-ttu-id="331f1-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="331f1-142">The following is a JSON representation of the resource.</span></span>

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


