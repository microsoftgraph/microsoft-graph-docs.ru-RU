---
title: Тип ресурса Акцесспаккажересаурцеролескопе
description: Область применения роли пакета Access — это ссылка на область в ресурсе и роль в этом ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4f10d297e59f9665d493060362a27e1c4b11a5a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938914"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="31b8b-103">Тип ресурса Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="31b8b-103">accessPackageResourceRoleScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31b8b-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)областью применения роли ресурса Package является ссылка на область в ресурсе и роль в этом ресурсе.</span><span class="sxs-lookup"><span data-stu-id="31b8b-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource.</span></span>

## <a name="properties"></a><span data-ttu-id="31b8b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="31b8b-105">Properties</span></span>

| <span data-ttu-id="31b8b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="31b8b-106">Property</span></span>     | <span data-ttu-id="31b8b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="31b8b-107">Type</span></span>        | <span data-ttu-id="31b8b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="31b8b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31b8b-109">createdBy</span><span class="sxs-lookup"><span data-stu-id="31b8b-109">createdBy</span></span>|<span data-ttu-id="31b8b-110">String</span><span class="sxs-lookup"><span data-stu-id="31b8b-110">String</span></span>|<span data-ttu-id="31b8b-111">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31b8b-111">Read-only.</span></span>|
|<span data-ttu-id="31b8b-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31b8b-112">createdDateTime</span></span>|<span data-ttu-id="31b8b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31b8b-113">DateTimeOffset</span></span>|<span data-ttu-id="31b8b-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="31b8b-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="31b8b-116">id</span><span class="sxs-lookup"><span data-stu-id="31b8b-116">id</span></span>|<span data-ttu-id="31b8b-117">String</span><span class="sxs-lookup"><span data-stu-id="31b8b-117">String</span></span>| <span data-ttu-id="31b8b-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31b8b-118">Read-only.</span></span>|
|<span data-ttu-id="31b8b-119">модифиедби</span><span class="sxs-lookup"><span data-stu-id="31b8b-119">modifiedBy</span></span>|<span data-ttu-id="31b8b-120">String</span><span class="sxs-lookup"><span data-stu-id="31b8b-120">String</span></span>|<span data-ttu-id="31b8b-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31b8b-121">Read-only.</span></span>|
|<span data-ttu-id="31b8b-122">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31b8b-122">modifiedDateTime</span></span>|<span data-ttu-id="31b8b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31b8b-123">DateTimeOffset</span></span>|<span data-ttu-id="31b8b-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="31b8b-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="31b8b-126">Связи</span><span class="sxs-lookup"><span data-stu-id="31b8b-126">Relationships</span></span>

| <span data-ttu-id="31b8b-127">Связь</span><span class="sxs-lookup"><span data-stu-id="31b8b-127">Relationship</span></span> | <span data-ttu-id="31b8b-128">Тип</span><span class="sxs-lookup"><span data-stu-id="31b8b-128">Type</span></span>        | <span data-ttu-id="31b8b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="31b8b-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="31b8b-130">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="31b8b-130">accessPackageResourceRole</span></span>|[<span data-ttu-id="31b8b-131">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="31b8b-131">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="31b8b-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31b8b-132">Read-only.</span></span> <span data-ttu-id="31b8b-133">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="31b8b-133">Nullable.</span></span>|
|<span data-ttu-id="31b8b-134">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="31b8b-134">accessPackageResourceScope</span></span>|[<span data-ttu-id="31b8b-135">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="31b8b-135">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="31b8b-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="31b8b-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31b8b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31b8b-138">JSON representation</span></span>

<span data-ttu-id="31b8b-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31b8b-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
