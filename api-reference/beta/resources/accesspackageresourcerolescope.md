---
title: Тип ресурса Акцесспаккажересаурцеролескопе
description: Область применения роли пакета Access — это ссылка на область в ресурсе и роль в этом ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c96d5a0499ae269c7ce67bae2252c6521d66eb7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024649"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="9de0f-103">Тип ресурса Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="9de0f-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="9de0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9de0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9de0f-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)областью применения роли ресурса Package является ссылка на область в ресурсе и роль в этом ресурсе для этой области.</span><span class="sxs-lookup"><span data-stu-id="9de0f-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="9de0f-106">Пакет Access будет иметь доступ к областям роли ресурса пакета для ресурсов в каталоге, которые относятся к этому пакету Access.</span><span class="sxs-lookup"><span data-stu-id="9de0f-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="9de0f-107">Когда тема получает назначение пакета Access, тема будет подготовлена к работе с ролью в этой области каждой области применения роли ресурса пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9de0f-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="9de0f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9de0f-108">Methods</span></span>

| <span data-ttu-id="9de0f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9de0f-109">Method</span></span>       | <span data-ttu-id="9de0f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9de0f-110">Return Type</span></span> | <span data-ttu-id="9de0f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9de0f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9de0f-112">Список Акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="9de0f-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="9de0f-113">Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="9de0f-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="9de0f-114">Получение списка объектов **акцесспаккажересаурцеролескопе** для пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9de0f-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="9de0f-115">Создание Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="9de0f-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="9de0f-116">Создайте новый объект **акцесспаккажересаурцеролескопе** для пакета Access.</span><span class="sxs-lookup"><span data-stu-id="9de0f-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="9de0f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9de0f-117">Properties</span></span>

| <span data-ttu-id="9de0f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9de0f-118">Property</span></span>     | <span data-ttu-id="9de0f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9de0f-119">Type</span></span>        | <span data-ttu-id="9de0f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9de0f-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9de0f-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="9de0f-121">createdBy</span></span>|<span data-ttu-id="9de0f-122">String</span><span class="sxs-lookup"><span data-stu-id="9de0f-122">String</span></span>|<span data-ttu-id="9de0f-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9de0f-123">Read-only.</span></span>|
|<span data-ttu-id="9de0f-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9de0f-124">createdDateTime</span></span>|<span data-ttu-id="9de0f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9de0f-125">DateTimeOffset</span></span>|<span data-ttu-id="9de0f-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9de0f-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9de0f-128">id</span><span class="sxs-lookup"><span data-stu-id="9de0f-128">id</span></span>|<span data-ttu-id="9de0f-129">String</span><span class="sxs-lookup"><span data-stu-id="9de0f-129">String</span></span>| <span data-ttu-id="9de0f-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9de0f-130">Read-only.</span></span>|
|<span data-ttu-id="9de0f-131">модифиедби</span><span class="sxs-lookup"><span data-stu-id="9de0f-131">modifiedBy</span></span>|<span data-ttu-id="9de0f-132">String</span><span class="sxs-lookup"><span data-stu-id="9de0f-132">String</span></span>|<span data-ttu-id="9de0f-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9de0f-133">Read-only.</span></span>|
|<span data-ttu-id="9de0f-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9de0f-134">modifiedDateTime</span></span>|<span data-ttu-id="9de0f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9de0f-135">DateTimeOffset</span></span>|<span data-ttu-id="9de0f-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9de0f-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="9de0f-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="9de0f-138">Relationships</span></span>

| <span data-ttu-id="9de0f-139">Связь</span><span class="sxs-lookup"><span data-stu-id="9de0f-139">Relationship</span></span> | <span data-ttu-id="9de0f-140">Тип</span><span class="sxs-lookup"><span data-stu-id="9de0f-140">Type</span></span>        | <span data-ttu-id="9de0f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="9de0f-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9de0f-142">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="9de0f-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="9de0f-143">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="9de0f-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="9de0f-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9de0f-144">Read-only.</span></span> <span data-ttu-id="9de0f-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9de0f-145">Nullable.</span></span>|
|<span data-ttu-id="9de0f-146">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="9de0f-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="9de0f-147">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="9de0f-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="9de0f-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9de0f-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9de0f-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9de0f-150">JSON representation</span></span>

<span data-ttu-id="9de0f-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9de0f-151">The following is a JSON representation of the resource.</span></span>

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
  "modifiedDateTime": "String (timestamp)",
  "accessPackageResourceRole": {
    "id": "String (identifier)",
     "displayName": "String",
     "originSystem": "String",
     "originId": "String"
  },
  "accessPackageResourceScope": {
     "id": "String (identifier)",
     "displayName": "String",
     "description": "String",
     "originId": "String (identifier)",
     "originSystem": "String"
  }

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


