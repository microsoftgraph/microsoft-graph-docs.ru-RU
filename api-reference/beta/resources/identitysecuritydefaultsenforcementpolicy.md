---
title: тип ресурса identitySecurityDefaultsEnforcementPolicy
description: Представляет политику безопасности по умолчанию Azure Active Directory. По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b06fd0b88a87dabb5a12e09b788094b8e00b8960
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440257"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="d0f33-104">тип ресурса identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="d0f33-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="d0f33-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f33-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0f33-106">Представляет политику безопасности по умолчанию Azure Active [Directory.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="d0f33-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="d0f33-107">По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="d0f33-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="d0f33-108">Наследует [от policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="d0f33-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d0f33-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d0f33-109">Methods</span></span>

| <span data-ttu-id="d0f33-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d0f33-110">Method</span></span>       | <span data-ttu-id="d0f33-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d0f33-111">Return Type</span></span> | <span data-ttu-id="d0f33-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d0f33-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d0f33-113">[получение](../api/identitysecuritydefaultsenforcementpolicy-get.md);</span><span class="sxs-lookup"><span data-stu-id="d0f33-113">[Get](../api/identitysecuritydefaultsenforcementpolicy-get.md)</span></span> | [<span data-ttu-id="d0f33-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="d0f33-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="d0f33-115">Ознакомьтесь с свойствами **объекта identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="d0f33-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="d0f33-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="d0f33-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="d0f33-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="d0f33-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="d0f33-118">Обновление **объекта identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="d0f33-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0f33-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0f33-119">Properties</span></span>

| <span data-ttu-id="d0f33-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0f33-120">Property</span></span>     | <span data-ttu-id="d0f33-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d0f33-121">Type</span></span>        | <span data-ttu-id="d0f33-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d0f33-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0f33-123">description</span><span class="sxs-lookup"><span data-stu-id="d0f33-123">description</span></span>|<span data-ttu-id="d0f33-124">String</span><span class="sxs-lookup"><span data-stu-id="d0f33-124">String</span></span>|<span data-ttu-id="d0f33-125">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0f33-125">Description for this policy.</span></span> <span data-ttu-id="d0f33-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0f33-126">Read-only.</span></span>|
|<span data-ttu-id="d0f33-127">displayName</span><span class="sxs-lookup"><span data-stu-id="d0f33-127">displayName</span></span>|<span data-ttu-id="d0f33-128">String</span><span class="sxs-lookup"><span data-stu-id="d0f33-128">String</span></span>|<span data-ttu-id="d0f33-129">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0f33-129">Display name for this policy.</span></span> <span data-ttu-id="d0f33-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0f33-130">Read-only.</span></span>|
|<span data-ttu-id="d0f33-131">id</span><span class="sxs-lookup"><span data-stu-id="d0f33-131">id</span></span>|<span data-ttu-id="d0f33-132">String</span><span class="sxs-lookup"><span data-stu-id="d0f33-132">String</span></span>|<span data-ttu-id="d0f33-133">Идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0f33-133">Identifier for this policy.</span></span> <span data-ttu-id="d0f33-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0f33-134">Read-only.</span></span>|
|<span data-ttu-id="d0f33-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d0f33-135">isEnabled</span></span>|<span data-ttu-id="d0f33-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0f33-136">Boolean</span></span>|<span data-ttu-id="d0f33-137">Если установлено значение true, по умолчанию безопасность Azure Active Directory включена для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0f33-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0f33-138">Связи</span><span class="sxs-lookup"><span data-stu-id="d0f33-138">Relationships</span></span>

<span data-ttu-id="d0f33-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d0f33-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0f33-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d0f33-140">JSON representation</span></span>

<span data-ttu-id="d0f33-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0f33-141">The following is a JSON representation of the resource.</span></span>

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
