---
title: Тип ресурса Акцесспаккажересаурцероле
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b5ab0cc6e2179adb62316cbcdc06b7dd52abc439
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508515"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="a4478-103">Тип ресурса Акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="a4478-103">accessPackageResourceRole resource type</span></span>

<span data-ttu-id="a4478-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4478-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4478-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета Access — это ссылка на роль, определенную в ресурсе, которую можно использовать в пакете Access.</span><span class="sxs-lookup"><span data-stu-id="a4478-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="methods"></a><span data-ttu-id="a4478-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a4478-106">Methods</span></span>

| <span data-ttu-id="a4478-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a4478-107">Method</span></span>       | <span data-ttu-id="a4478-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4478-108">Return Type</span></span> | <span data-ttu-id="a4478-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4478-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a4478-110">Список ролей ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="a4478-110">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="a4478-111">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="a4478-111">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="a4478-112">Получение списка объектов Акцесспаккажересаурцероле для каталога.</span><span class="sxs-lookup"><span data-stu-id="a4478-112">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4478-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4478-113">Properties</span></span>

| <span data-ttu-id="a4478-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4478-114">Property</span></span>     | <span data-ttu-id="a4478-115">Тип</span><span class="sxs-lookup"><span data-stu-id="a4478-115">Type</span></span>        | <span data-ttu-id="a4478-116">Описание</span><span class="sxs-lookup"><span data-stu-id="a4478-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4478-117">description</span><span class="sxs-lookup"><span data-stu-id="a4478-117">description</span></span>|<span data-ttu-id="a4478-118">String</span><span class="sxs-lookup"><span data-stu-id="a4478-118">String</span></span>|<span data-ttu-id="a4478-119">Описание роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="a4478-119">A description for the resource role.</span></span>|
|<span data-ttu-id="a4478-120">displayName</span><span class="sxs-lookup"><span data-stu-id="a4478-120">displayName</span></span>|<span data-ttu-id="a4478-121">Строка</span><span class="sxs-lookup"><span data-stu-id="a4478-121">String</span></span>|<span data-ttu-id="a4478-122">Отображаемое имя роли ресурса, например роль, определяемую приложением.</span><span class="sxs-lookup"><span data-stu-id="a4478-122">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="a4478-123">id</span><span class="sxs-lookup"><span data-stu-id="a4478-123">id</span></span>|<span data-ttu-id="a4478-124">String</span><span class="sxs-lookup"><span data-stu-id="a4478-124">String</span></span>| <span data-ttu-id="a4478-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4478-125">Read-only.</span></span>|
|<span data-ttu-id="a4478-126">оригинид</span><span class="sxs-lookup"><span data-stu-id="a4478-126">originId</span></span>|<span data-ttu-id="a4478-127">String</span><span class="sxs-lookup"><span data-stu-id="a4478-127">String</span></span>|<span data-ttu-id="a4478-128">Уникальный идентификатор роли ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="a4478-128">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="a4478-129">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="a4478-129">originSystem</span></span>|<span data-ttu-id="a4478-130">String</span><span class="sxs-lookup"><span data-stu-id="a4478-130">String</span></span>|<span data-ttu-id="a4478-131">Тип ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="a4478-131">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4478-132">Связи</span><span class="sxs-lookup"><span data-stu-id="a4478-132">Relationships</span></span>

| <span data-ttu-id="a4478-133">Связь</span><span class="sxs-lookup"><span data-stu-id="a4478-133">Relationship</span></span> | <span data-ttu-id="a4478-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a4478-134">Type</span></span>        | <span data-ttu-id="a4478-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a4478-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4478-136">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="a4478-136">accessPackageResource</span></span>|[<span data-ttu-id="a4478-137">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="a4478-137">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="a4478-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a4478-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4478-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4478-140">JSON representation</span></span>

<span data-ttu-id="a4478-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4478-141">The following is a JSON representation of the resource.</span></span>

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
