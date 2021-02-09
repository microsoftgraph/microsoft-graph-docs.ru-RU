---
title: Тип ресурса identitySecurityDefaultsEnforcementPolicy
description: Представляет политику по умолчанию для безопасности Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно заранее задав параметры безопасности, которые защищают от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1dea4d94dfc8de8310410498fdf8d83c2a5e8f68
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154931"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="3fe85-104">Тип ресурса identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="3fe85-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="3fe85-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fe85-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fe85-106">Представляет политику по умолчанию для [безопасности](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3fe85-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="3fe85-107">Значения по умолчанию для системы безопасности содержат предварительно заранее настраиваемую настройку параметров безопасности, которые защищают от распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="3fe85-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="3fe85-108">Наследуется [от policyBase.](../resources/policybase.md)</span><span class="sxs-lookup"><span data-stu-id="3fe85-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3fe85-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3fe85-109">Methods</span></span>

| <span data-ttu-id="3fe85-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3fe85-110">Method</span></span>       | <span data-ttu-id="3fe85-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3fe85-111">Return Type</span></span> | <span data-ttu-id="3fe85-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3fe85-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3fe85-113">Получение</span><span class="sxs-lookup"><span data-stu-id="3fe85-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="3fe85-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="3fe85-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="3fe85-115">Чтение свойств объекта **identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="3fe85-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="3fe85-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="3fe85-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="3fe85-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="3fe85-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="3fe85-118">Обновление объекта **identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="3fe85-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3fe85-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fe85-119">Properties</span></span>

| <span data-ttu-id="3fe85-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fe85-120">Property</span></span>     | <span data-ttu-id="3fe85-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3fe85-121">Type</span></span>        | <span data-ttu-id="3fe85-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3fe85-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3fe85-123">description</span><span class="sxs-lookup"><span data-stu-id="3fe85-123">description</span></span>|<span data-ttu-id="3fe85-124">String</span><span class="sxs-lookup"><span data-stu-id="3fe85-124">String</span></span>|<span data-ttu-id="3fe85-125">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="3fe85-125">Description for this policy.</span></span> <span data-ttu-id="3fe85-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fe85-126">Read-only.</span></span>|
|<span data-ttu-id="3fe85-127">displayName</span><span class="sxs-lookup"><span data-stu-id="3fe85-127">displayName</span></span>|<span data-ttu-id="3fe85-128">String</span><span class="sxs-lookup"><span data-stu-id="3fe85-128">String</span></span>|<span data-ttu-id="3fe85-129">Отображаемого имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3fe85-129">Display name for this policy.</span></span> <span data-ttu-id="3fe85-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fe85-130">Read-only.</span></span>|
|<span data-ttu-id="3fe85-131">id</span><span class="sxs-lookup"><span data-stu-id="3fe85-131">id</span></span>|<span data-ttu-id="3fe85-132">String</span><span class="sxs-lookup"><span data-stu-id="3fe85-132">String</span></span>|<span data-ttu-id="3fe85-133">Идентификатор этой политики.</span><span class="sxs-lookup"><span data-stu-id="3fe85-133">Identifier for this policy.</span></span> <span data-ttu-id="3fe85-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fe85-134">Read-only.</span></span>|
|<span data-ttu-id="3fe85-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3fe85-135">isEnabled</span></span>|<span data-ttu-id="3fe85-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fe85-136">Boolean</span></span>|<span data-ttu-id="3fe85-137">Если установлено значение true, для клиента включены значения по умолчанию для системы безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3fe85-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fe85-138">Связи</span><span class="sxs-lookup"><span data-stu-id="3fe85-138">Relationships</span></span>

<span data-ttu-id="3fe85-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3fe85-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fe85-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3fe85-140">JSON representation</span></span>

<span data-ttu-id="3fe85-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fe85-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySecurityDefaultsEnforcementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->