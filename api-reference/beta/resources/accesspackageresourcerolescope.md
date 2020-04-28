---
title: Тип ресурса Акцесспаккажересаурцеролескопе
description: Область применения роли пакета Access — это ссылка на область в ресурсе и роль в этом ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719f2ac275a19c9e4cef4cb2403166933e2e5925
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508508"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="325ab-103">Тип ресурса Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="325ab-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="325ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="325ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="325ab-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)областью применения роли ресурса Package является ссылка на область в ресурсе и роль в этом ресурсе для этой области.</span><span class="sxs-lookup"><span data-stu-id="325ab-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="325ab-106">Пакет Access будет иметь доступ к областям роли ресурса пакета для ресурсов в каталоге, которые относятся к этому пакету Access.</span><span class="sxs-lookup"><span data-stu-id="325ab-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="325ab-107">Когда тема получает назначение пакета Access, тема будет подготовлена к работе с ролью в этой области каждой области применения роли ресурса пакета Access.</span><span class="sxs-lookup"><span data-stu-id="325ab-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="325ab-108">Методы</span><span class="sxs-lookup"><span data-stu-id="325ab-108">Methods</span></span>

| <span data-ttu-id="325ab-109">Метод</span><span class="sxs-lookup"><span data-stu-id="325ab-109">Method</span></span>       | <span data-ttu-id="325ab-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="325ab-110">Return Type</span></span> | <span data-ttu-id="325ab-111">Описание</span><span class="sxs-lookup"><span data-stu-id="325ab-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="325ab-112">Список Акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="325ab-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="325ab-113">Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="325ab-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="325ab-114">Получение списка объектов **акцесспаккажересаурцеролескопе** для пакета Access.</span><span class="sxs-lookup"><span data-stu-id="325ab-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="325ab-115">Создание Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="325ab-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="325ab-116">Создайте новый объект **акцесспаккажересаурцеролескопе** для пакета Access.</span><span class="sxs-lookup"><span data-stu-id="325ab-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="325ab-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="325ab-117">Properties</span></span>

| <span data-ttu-id="325ab-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="325ab-118">Property</span></span>     | <span data-ttu-id="325ab-119">Тип</span><span class="sxs-lookup"><span data-stu-id="325ab-119">Type</span></span>        | <span data-ttu-id="325ab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="325ab-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="325ab-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="325ab-121">createdBy</span></span>|<span data-ttu-id="325ab-122">String</span><span class="sxs-lookup"><span data-stu-id="325ab-122">String</span></span>|<span data-ttu-id="325ab-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="325ab-123">Read-only.</span></span>|
|<span data-ttu-id="325ab-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="325ab-124">createdDateTime</span></span>|<span data-ttu-id="325ab-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="325ab-125">DateTimeOffset</span></span>|<span data-ttu-id="325ab-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="325ab-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="325ab-128">id</span><span class="sxs-lookup"><span data-stu-id="325ab-128">id</span></span>|<span data-ttu-id="325ab-129">String</span><span class="sxs-lookup"><span data-stu-id="325ab-129">String</span></span>| <span data-ttu-id="325ab-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="325ab-130">Read-only.</span></span>|
|<span data-ttu-id="325ab-131">модифиедби</span><span class="sxs-lookup"><span data-stu-id="325ab-131">modifiedBy</span></span>|<span data-ttu-id="325ab-132">String</span><span class="sxs-lookup"><span data-stu-id="325ab-132">String</span></span>|<span data-ttu-id="325ab-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="325ab-133">Read-only.</span></span>|
|<span data-ttu-id="325ab-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="325ab-134">modifiedDateTime</span></span>|<span data-ttu-id="325ab-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="325ab-135">DateTimeOffset</span></span>|<span data-ttu-id="325ab-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="325ab-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="325ab-138">Связи</span><span class="sxs-lookup"><span data-stu-id="325ab-138">Relationships</span></span>

| <span data-ttu-id="325ab-139">Связь</span><span class="sxs-lookup"><span data-stu-id="325ab-139">Relationship</span></span> | <span data-ttu-id="325ab-140">Тип</span><span class="sxs-lookup"><span data-stu-id="325ab-140">Type</span></span>        | <span data-ttu-id="325ab-141">Описание</span><span class="sxs-lookup"><span data-stu-id="325ab-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="325ab-142">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="325ab-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="325ab-143">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="325ab-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="325ab-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="325ab-144">Read-only.</span></span> <span data-ttu-id="325ab-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="325ab-145">Nullable.</span></span>|
|<span data-ttu-id="325ab-146">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="325ab-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="325ab-147">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="325ab-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="325ab-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="325ab-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="325ab-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="325ab-150">JSON representation</span></span>

<span data-ttu-id="325ab-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="325ab-151">The following is a JSON representation of the resource.</span></span>

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
