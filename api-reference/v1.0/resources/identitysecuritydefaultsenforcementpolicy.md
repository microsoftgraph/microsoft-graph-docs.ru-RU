---
title: тип ресурса identitySecurityDefaultsEnforcementPolicy
description: Представляет политику безопасности по умолчанию Azure Active Directory. По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 21b012338e6ca168e932a8aaf2560ce825304ae9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439844"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="0ab7b-104">тип ресурса identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="0ab7b-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="0ab7b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ab7b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0ab7b-106">Представляет политику безопасности по умолчанию Azure Active [Directory.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="0ab7b-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="0ab7b-107">По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="0ab7b-108">Наследует [от policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="0ab7b-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0ab7b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0ab7b-109">Methods</span></span>

| <span data-ttu-id="0ab7b-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0ab7b-110">Method</span></span>       | <span data-ttu-id="0ab7b-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0ab7b-111">Return Type</span></span> | <span data-ttu-id="0ab7b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0ab7b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0ab7b-113">Получение</span><span class="sxs-lookup"><span data-stu-id="0ab7b-113">Get</span></span>](../api/identitysecuritydefaultsenforcementpolicy-get.md) | [<span data-ttu-id="0ab7b-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="0ab7b-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="0ab7b-115">Ознакомьтесь с свойствами **объекта identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="0ab7b-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="0ab7b-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="0ab7b-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="0ab7b-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="0ab7b-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="0ab7b-118">Обновление **объекта identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="0ab7b-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0ab7b-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ab7b-119">Properties</span></span>

| <span data-ttu-id="0ab7b-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ab7b-120">Property</span></span>     | <span data-ttu-id="0ab7b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0ab7b-121">Type</span></span>        | <span data-ttu-id="0ab7b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0ab7b-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ab7b-123">description</span><span class="sxs-lookup"><span data-stu-id="0ab7b-123">description</span></span>|<span data-ttu-id="0ab7b-124">String</span><span class="sxs-lookup"><span data-stu-id="0ab7b-124">String</span></span>|<span data-ttu-id="0ab7b-125">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-125">Description for this policy.</span></span> <span data-ttu-id="0ab7b-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-126">Read-only.</span></span>|
|<span data-ttu-id="0ab7b-127">displayName</span><span class="sxs-lookup"><span data-stu-id="0ab7b-127">displayName</span></span>|<span data-ttu-id="0ab7b-128">String</span><span class="sxs-lookup"><span data-stu-id="0ab7b-128">String</span></span>|<span data-ttu-id="0ab7b-129">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-129">Display name for this policy.</span></span> <span data-ttu-id="0ab7b-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-130">Read-only.</span></span>|
|<span data-ttu-id="0ab7b-131">id</span><span class="sxs-lookup"><span data-stu-id="0ab7b-131">id</span></span>|<span data-ttu-id="0ab7b-132">String</span><span class="sxs-lookup"><span data-stu-id="0ab7b-132">String</span></span>|<span data-ttu-id="0ab7b-133">Идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-133">Identifier for this policy.</span></span> <span data-ttu-id="0ab7b-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-134">Read-only.</span></span>|
|<span data-ttu-id="0ab7b-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0ab7b-135">isEnabled</span></span>|<span data-ttu-id="0ab7b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ab7b-136">Boolean</span></span>|<span data-ttu-id="0ab7b-137">Если установлено значение true, по умолчанию безопасность Azure Active Directory включена для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ab7b-138">Связи</span><span class="sxs-lookup"><span data-stu-id="0ab7b-138">Relationships</span></span>

<span data-ttu-id="0ab7b-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ab7b-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0ab7b-140">JSON representation</span></span>

<span data-ttu-id="0ab7b-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ab7b-141">The following is a JSON representation of the resource.</span></span>

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
