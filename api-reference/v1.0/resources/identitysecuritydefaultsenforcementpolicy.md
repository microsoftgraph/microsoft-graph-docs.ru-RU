---
title: Тип ресурса Идентитисекуритидефаултсенфорцементполици
description: Представляет политику безопасности по умолчанию для Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c208733525162397c190bd425cdf7c770a302c0f
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581920"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="c5e9d-104">Тип ресурса Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="c5e9d-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="c5e9d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5e9d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c5e9d-106">Представляет политику [безопасности по умолчанию](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="c5e9d-107">Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="c5e9d-108">Наследуется от [основы](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="c5e9d-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c5e9d-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c5e9d-109">Methods</span></span>

| <span data-ttu-id="c5e9d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c5e9d-110">Method</span></span>       | <span data-ttu-id="c5e9d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c5e9d-111">Return Type</span></span> | <span data-ttu-id="c5e9d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c5e9d-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c5e9d-113">[получение](../api/identitysecuritydefaultsenforcementpolicy-get.md);</span><span class="sxs-lookup"><span data-stu-id="c5e9d-113">[Get](../api/identitysecuritydefaultsenforcementpolicy-get.md)</span></span> | [<span data-ttu-id="c5e9d-114">идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="c5e9d-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="c5e9d-115">Чтение свойств объекта **идентитисекуритидефаултсенфорцементполици** .</span><span class="sxs-lookup"><span data-stu-id="c5e9d-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| <span data-ttu-id="c5e9d-116">[обновление](../api/identitysecuritydefaultsenforcementpolicy-update.md).</span><span class="sxs-lookup"><span data-stu-id="c5e9d-116">[Update](../api/identitysecuritydefaultsenforcementpolicy-update.md)</span></span> | [<span data-ttu-id="c5e9d-117">идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="c5e9d-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="c5e9d-118">Обновление объекта **идентитисекуритидефаултсенфорцементполици** .</span><span class="sxs-lookup"><span data-stu-id="c5e9d-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c5e9d-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5e9d-119">Properties</span></span>

| <span data-ttu-id="c5e9d-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5e9d-120">Property</span></span>     | <span data-ttu-id="c5e9d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c5e9d-121">Type</span></span>        | <span data-ttu-id="c5e9d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c5e9d-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c5e9d-123">description</span><span class="sxs-lookup"><span data-stu-id="c5e9d-123">description</span></span>|<span data-ttu-id="c5e9d-124">String</span><span class="sxs-lookup"><span data-stu-id="c5e9d-124">String</span></span>|<span data-ttu-id="c5e9d-125">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-125">Description for this policy.</span></span> <span data-ttu-id="c5e9d-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-126">Read-only.</span></span>|
|<span data-ttu-id="c5e9d-127">displayName</span><span class="sxs-lookup"><span data-stu-id="c5e9d-127">displayName</span></span>|<span data-ttu-id="c5e9d-128">String</span><span class="sxs-lookup"><span data-stu-id="c5e9d-128">String</span></span>|<span data-ttu-id="c5e9d-129">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-129">Display name for this policy.</span></span> <span data-ttu-id="c5e9d-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-130">Read-only.</span></span>|
|<span data-ttu-id="c5e9d-131">id</span><span class="sxs-lookup"><span data-stu-id="c5e9d-131">id</span></span>|<span data-ttu-id="c5e9d-132">String</span><span class="sxs-lookup"><span data-stu-id="c5e9d-132">String</span></span>|<span data-ttu-id="c5e9d-133">Идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-133">Identifier for this policy.</span></span> <span data-ttu-id="c5e9d-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-134">Read-only.</span></span>|
|<span data-ttu-id="c5e9d-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c5e9d-135">isEnabled</span></span>|<span data-ttu-id="c5e9d-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5e9d-136">Boolean</span></span>|<span data-ttu-id="c5e9d-137">Если задано значение true, по умолчанию для клиента будет включен параметр безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5e9d-138">Связи</span><span class="sxs-lookup"><span data-stu-id="c5e9d-138">Relationships</span></span>

<span data-ttu-id="c5e9d-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5e9d-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c5e9d-140">JSON representation</span></span>

<span data-ttu-id="c5e9d-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5e9d-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "baseType": "",
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