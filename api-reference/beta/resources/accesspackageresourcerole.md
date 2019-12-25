---
title: Тип ресурса Акцесспаккажересаурцероле
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 21cda352cb887a377248a3fbbf16a761773128ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870428"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="1010e-103">Тип ресурса Акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="1010e-103">accessPackageResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1010e-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета Access — это ссылка на роль, определенную в ресурсе, которую можно использовать в пакете Access.</span><span class="sxs-lookup"><span data-stu-id="1010e-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="methods"></a><span data-ttu-id="1010e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1010e-105">Methods</span></span>

| <span data-ttu-id="1010e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1010e-106">Method</span></span>       | <span data-ttu-id="1010e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1010e-107">Return Type</span></span> | <span data-ttu-id="1010e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1010e-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1010e-109">Список ролей ресурсов Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="1010e-109">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="1010e-110">Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="1010e-110">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="1010e-111">Получение списка объектов Акцесспаккажересаурцероле для каталога.</span><span class="sxs-lookup"><span data-stu-id="1010e-111">Retrieve a list of accessPackageResourceRole objects for a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="1010e-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="1010e-112">Properties</span></span>

| <span data-ttu-id="1010e-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="1010e-113">Property</span></span>     | <span data-ttu-id="1010e-114">Тип</span><span class="sxs-lookup"><span data-stu-id="1010e-114">Type</span></span>        | <span data-ttu-id="1010e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="1010e-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1010e-116">description</span><span class="sxs-lookup"><span data-stu-id="1010e-116">description</span></span>|<span data-ttu-id="1010e-117">String</span><span class="sxs-lookup"><span data-stu-id="1010e-117">String</span></span>|<span data-ttu-id="1010e-118">Описание роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="1010e-118">A description for the resource role.</span></span>|
|<span data-ttu-id="1010e-119">displayName</span><span class="sxs-lookup"><span data-stu-id="1010e-119">displayName</span></span>|<span data-ttu-id="1010e-120">Строка</span><span class="sxs-lookup"><span data-stu-id="1010e-120">String</span></span>|<span data-ttu-id="1010e-121">Отображаемое имя роли ресурса, например роль, определяемую приложением.</span><span class="sxs-lookup"><span data-stu-id="1010e-121">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="1010e-122">id</span><span class="sxs-lookup"><span data-stu-id="1010e-122">id</span></span>|<span data-ttu-id="1010e-123">String</span><span class="sxs-lookup"><span data-stu-id="1010e-123">String</span></span>| <span data-ttu-id="1010e-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1010e-124">Read-only.</span></span>|
|<span data-ttu-id="1010e-125">оригинид</span><span class="sxs-lookup"><span data-stu-id="1010e-125">originId</span></span>|<span data-ttu-id="1010e-126">String</span><span class="sxs-lookup"><span data-stu-id="1010e-126">String</span></span>|<span data-ttu-id="1010e-127">Уникальный идентификатор роли ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="1010e-127">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="1010e-128">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="1010e-128">originSystem</span></span>|<span data-ttu-id="1010e-129">String</span><span class="sxs-lookup"><span data-stu-id="1010e-129">String</span></span>|<span data-ttu-id="1010e-130">Тип ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="1010e-130">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1010e-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="1010e-131">Relationships</span></span>

| <span data-ttu-id="1010e-132">Связь</span><span class="sxs-lookup"><span data-stu-id="1010e-132">Relationship</span></span> | <span data-ttu-id="1010e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1010e-133">Type</span></span>        | <span data-ttu-id="1010e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1010e-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1010e-135">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="1010e-135">accessPackageResource</span></span>|[<span data-ttu-id="1010e-136">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="1010e-136">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="1010e-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1010e-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1010e-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1010e-139">JSON representation</span></span>

<span data-ttu-id="1010e-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1010e-140">The following is a JSON representation of the resource.</span></span>

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
