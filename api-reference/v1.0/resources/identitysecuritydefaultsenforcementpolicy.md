---
title: тип ресурса identitySecurityDefaultsEnforcementPolicy
description: Представляет политику безопасности по умолчанию Azure Active Directory. По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2609a75ad90aba9ab545e81207bc0d3ea33f0a8a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944845"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="395c4-104">тип ресурса identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="395c4-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="395c4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="395c4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="395c4-106">Представляет политику безопасности по умолчанию Azure Active [Directory.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="395c4-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="395c4-107">По умолчанию в безопасности содержатся преднастройные параметры безопасности, защищающие от распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="395c4-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="395c4-108">Наследует [от policyBase](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="395c4-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="395c4-109">Методы</span><span class="sxs-lookup"><span data-stu-id="395c4-109">Methods</span></span>

| <span data-ttu-id="395c4-110">Метод</span><span class="sxs-lookup"><span data-stu-id="395c4-110">Method</span></span>       | <span data-ttu-id="395c4-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="395c4-111">Return Type</span></span> | <span data-ttu-id="395c4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="395c4-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="395c4-113">[получение](../api/identitysecuritydefaultsenforcementpolicy-get.md);</span><span class="sxs-lookup"><span data-stu-id="395c4-113">[Get](../api/identitysecuritydefaultsenforcementpolicy-get.md)</span></span> | [<span data-ttu-id="395c4-114">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="395c4-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="395c4-115">Ознакомьтесь с свойствами **объекта identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="395c4-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| [<span data-ttu-id="395c4-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="395c4-116">Update</span></span>](../api/identitysecuritydefaultsenforcementpolicy-update.md) | [<span data-ttu-id="395c4-117">identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="395c4-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="395c4-118">Обновление **объекта identitySecurityDefaultsEnforcementPolicy.**</span><span class="sxs-lookup"><span data-stu-id="395c4-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="395c4-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="395c4-119">Properties</span></span>

| <span data-ttu-id="395c4-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="395c4-120">Property</span></span>     | <span data-ttu-id="395c4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="395c4-121">Type</span></span>        | <span data-ttu-id="395c4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="395c4-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="395c4-123">description</span><span class="sxs-lookup"><span data-stu-id="395c4-123">description</span></span>|<span data-ttu-id="395c4-124">Строка</span><span class="sxs-lookup"><span data-stu-id="395c4-124">String</span></span>|<span data-ttu-id="395c4-125">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="395c4-125">Description for this policy.</span></span> <span data-ttu-id="395c4-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="395c4-126">Read-only.</span></span>|
|<span data-ttu-id="395c4-127">displayName</span><span class="sxs-lookup"><span data-stu-id="395c4-127">displayName</span></span>|<span data-ttu-id="395c4-128">Строка</span><span class="sxs-lookup"><span data-stu-id="395c4-128">String</span></span>|<span data-ttu-id="395c4-129">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="395c4-129">Display name for this policy.</span></span> <span data-ttu-id="395c4-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="395c4-130">Read-only.</span></span>|
|<span data-ttu-id="395c4-131">id</span><span class="sxs-lookup"><span data-stu-id="395c4-131">id</span></span>|<span data-ttu-id="395c4-132">Строка</span><span class="sxs-lookup"><span data-stu-id="395c4-132">String</span></span>|<span data-ttu-id="395c4-133">Идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="395c4-133">Identifier for this policy.</span></span> <span data-ttu-id="395c4-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="395c4-134">Read-only.</span></span>|
|<span data-ttu-id="395c4-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="395c4-135">isEnabled</span></span>|<span data-ttu-id="395c4-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="395c4-136">Boolean</span></span>|<span data-ttu-id="395c4-137">Если установлено значение, по умолчанию `true` безопасность Azure Active Directory включена для клиента.</span><span class="sxs-lookup"><span data-stu-id="395c4-137">If set to `true`, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="395c4-138">Связи</span><span class="sxs-lookup"><span data-stu-id="395c4-138">Relationships</span></span>

<span data-ttu-id="395c4-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="395c4-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="395c4-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="395c4-140">JSON representation</span></span>

<span data-ttu-id="395c4-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="395c4-141">The following is a JSON representation of the resource.</span></span>

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
