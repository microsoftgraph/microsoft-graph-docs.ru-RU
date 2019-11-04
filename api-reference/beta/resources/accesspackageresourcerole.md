---
title: Тип ресурса Акцесспаккажересаурцероле
description: Ссылка на роль, определенную в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b5ae5d321ac5fec86801ca11f60ead8a276fd73
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938921"
---
# <a name="accesspackageresourcerole-resource-type"></a><span data-ttu-id="b59b5-103">Тип ресурса Акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="b59b5-103">accessPackageResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b59b5-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)роль ресурса пакета Access — это ссылка на роль, определенную в ресурсе, которую можно использовать в пакете Access.</span><span class="sxs-lookup"><span data-stu-id="b59b5-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role is a reference to a role defined in a resource, that can be used in an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="b59b5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b59b5-105">Properties</span></span>

| <span data-ttu-id="b59b5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b59b5-106">Property</span></span>     | <span data-ttu-id="b59b5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b59b5-107">Type</span></span>        | <span data-ttu-id="b59b5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b59b5-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b59b5-109">description</span><span class="sxs-lookup"><span data-stu-id="b59b5-109">description</span></span>|<span data-ttu-id="b59b5-110">String</span><span class="sxs-lookup"><span data-stu-id="b59b5-110">String</span></span>|<span data-ttu-id="b59b5-111">Описание роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="b59b5-111">A description for the resource role.</span></span>|
|<span data-ttu-id="b59b5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b59b5-112">displayName</span></span>|<span data-ttu-id="b59b5-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b59b5-113">String</span></span>|<span data-ttu-id="b59b5-114">Отображаемое имя роли ресурса, например роль, определяемую приложением.</span><span class="sxs-lookup"><span data-stu-id="b59b5-114">The display name of the resource role such as the role defined by the application.</span></span>|
|<span data-ttu-id="b59b5-115">id</span><span class="sxs-lookup"><span data-stu-id="b59b5-115">id</span></span>|<span data-ttu-id="b59b5-116">String</span><span class="sxs-lookup"><span data-stu-id="b59b5-116">String</span></span>| <span data-ttu-id="b59b5-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b59b5-117">Read-only.</span></span>|
|<span data-ttu-id="b59b5-118">оригинид</span><span class="sxs-lookup"><span data-stu-id="b59b5-118">originId</span></span>|<span data-ttu-id="b59b5-119">Строка</span><span class="sxs-lookup"><span data-stu-id="b59b5-119">String</span></span>|<span data-ttu-id="b59b5-120">Уникальный идентификатор роли ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="b59b5-120">The unique identifier of the resource role in the origin system.</span></span> |
|<span data-ttu-id="b59b5-121">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="b59b5-121">originSystem</span></span>|<span data-ttu-id="b59b5-122">Строка</span><span class="sxs-lookup"><span data-stu-id="b59b5-122">String</span></span>|<span data-ttu-id="b59b5-123">Тип ресурса в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="b59b5-123">The type of the resource in the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b59b5-124">Связи</span><span class="sxs-lookup"><span data-stu-id="b59b5-124">Relationships</span></span>

| <span data-ttu-id="b59b5-125">Связь</span><span class="sxs-lookup"><span data-stu-id="b59b5-125">Relationship</span></span> | <span data-ttu-id="b59b5-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b59b5-126">Type</span></span>        | <span data-ttu-id="b59b5-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b59b5-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b59b5-128">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="b59b5-128">accessPackageResource</span></span>|[<span data-ttu-id="b59b5-129">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="b59b5-129">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="b59b5-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b59b5-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b59b5-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b59b5-132">JSON representation</span></span>

<span data-ttu-id="b59b5-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b59b5-133">The following is a JSON representation of the resource.</span></span>

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
