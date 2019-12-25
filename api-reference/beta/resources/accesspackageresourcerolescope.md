---
title: Тип ресурса Акцесспаккажересаурцеролескопе
description: Область применения роли пакета Access — это ссылка на область в ресурсе и роль в этом ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ee4ec63c9c2efb60850ee7915e62dc0e284f8ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870964"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="83acb-103">Тип ресурса Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="83acb-103">accessPackageResourceRoleScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83acb-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)областью применения роли ресурса Package является ссылка на область в ресурсе и роль в этом ресурсе для этой области.</span><span class="sxs-lookup"><span data-stu-id="83acb-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="83acb-105">Пакет Access будет иметь доступ к областям роли ресурса пакета для ресурсов в каталоге, которые относятся к этому пакету Access.</span><span class="sxs-lookup"><span data-stu-id="83acb-105">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="83acb-106">Когда тема получает назначение пакета Access, тема будет подготовлена к работе с ролью в этой области каждой области применения роли ресурса пакета Access.</span><span class="sxs-lookup"><span data-stu-id="83acb-106">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="83acb-107">Методы</span><span class="sxs-lookup"><span data-stu-id="83acb-107">Methods</span></span>

| <span data-ttu-id="83acb-108">Метод</span><span class="sxs-lookup"><span data-stu-id="83acb-108">Method</span></span>       | <span data-ttu-id="83acb-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="83acb-109">Return Type</span></span> | <span data-ttu-id="83acb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="83acb-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="83acb-111">Список Акцесспаккажересаурцеролескопес</span><span class="sxs-lookup"><span data-stu-id="83acb-111">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="83acb-112">Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="83acb-112">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="83acb-113">Получение списка объектов **акцесспаккажересаурцеролескопе** для пакета Access.</span><span class="sxs-lookup"><span data-stu-id="83acb-113">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="83acb-114">Создание Акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="83acb-114">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="83acb-115">Создайте новый объект **акцесспаккажересаурцеролескопе** для пакета Access.</span><span class="sxs-lookup"><span data-stu-id="83acb-115">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="83acb-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="83acb-116">Properties</span></span>

| <span data-ttu-id="83acb-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="83acb-117">Property</span></span>     | <span data-ttu-id="83acb-118">Тип</span><span class="sxs-lookup"><span data-stu-id="83acb-118">Type</span></span>        | <span data-ttu-id="83acb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="83acb-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="83acb-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="83acb-120">createdBy</span></span>|<span data-ttu-id="83acb-121">String</span><span class="sxs-lookup"><span data-stu-id="83acb-121">String</span></span>|<span data-ttu-id="83acb-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83acb-122">Read-only.</span></span>|
|<span data-ttu-id="83acb-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83acb-123">createdDateTime</span></span>|<span data-ttu-id="83acb-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83acb-124">DateTimeOffset</span></span>|<span data-ttu-id="83acb-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="83acb-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="83acb-127">id</span><span class="sxs-lookup"><span data-stu-id="83acb-127">id</span></span>|<span data-ttu-id="83acb-128">String</span><span class="sxs-lookup"><span data-stu-id="83acb-128">String</span></span>| <span data-ttu-id="83acb-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83acb-129">Read-only.</span></span>|
|<span data-ttu-id="83acb-130">модифиедби</span><span class="sxs-lookup"><span data-stu-id="83acb-130">modifiedBy</span></span>|<span data-ttu-id="83acb-131">String</span><span class="sxs-lookup"><span data-stu-id="83acb-131">String</span></span>|<span data-ttu-id="83acb-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83acb-132">Read-only.</span></span>|
|<span data-ttu-id="83acb-133">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83acb-133">modifiedDateTime</span></span>|<span data-ttu-id="83acb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83acb-134">DateTimeOffset</span></span>|<span data-ttu-id="83acb-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="83acb-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="83acb-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="83acb-137">Relationships</span></span>

| <span data-ttu-id="83acb-138">Связь</span><span class="sxs-lookup"><span data-stu-id="83acb-138">Relationship</span></span> | <span data-ttu-id="83acb-139">Тип</span><span class="sxs-lookup"><span data-stu-id="83acb-139">Type</span></span>        | <span data-ttu-id="83acb-140">Описание</span><span class="sxs-lookup"><span data-stu-id="83acb-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="83acb-141">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="83acb-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="83acb-142">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="83acb-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="83acb-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83acb-143">Read-only.</span></span> <span data-ttu-id="83acb-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="83acb-144">Nullable.</span></span>|
|<span data-ttu-id="83acb-145">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="83acb-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="83acb-146">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="83acb-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="83acb-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="83acb-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83acb-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83acb-149">JSON representation</span></span>

<span data-ttu-id="83acb-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83acb-150">The following is a JSON representation of the resource.</span></span>

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
