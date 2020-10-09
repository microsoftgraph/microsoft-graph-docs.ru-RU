---
title: Тип ресурса Идентитисекуритидефаултсенфорцементполици
description: Представляет политику безопасности по умолчанию для Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d9e20693b6421573c13f696dbad837eda2f3619
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401388"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="4f959-104">Тип ресурса Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="4f959-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="4f959-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f959-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f959-106">Представляет политику [безопасности по умолчанию](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4f959-106">Represents the Azure Active Directory [security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="4f959-107">Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="4f959-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="4f959-108">Наследуется от [основы](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="4f959-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4f959-109">Методы</span><span class="sxs-lookup"><span data-stu-id="4f959-109">Methods</span></span>

| <span data-ttu-id="4f959-110">Метод</span><span class="sxs-lookup"><span data-stu-id="4f959-110">Method</span></span>       | <span data-ttu-id="4f959-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4f959-111">Return Type</span></span> | <span data-ttu-id="4f959-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4f959-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4f959-113">[получение](../api/identitysecuritydefaultsenforcementpolicy-get.md);</span><span class="sxs-lookup"><span data-stu-id="4f959-113">[Get](../api/identitysecuritydefaultsenforcementpolicy-get.md)</span></span> | [<span data-ttu-id="4f959-114">идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="4f959-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="4f959-115">Чтение свойств объекта **идентитисекуритидефаултсенфорцементполици** .</span><span class="sxs-lookup"><span data-stu-id="4f959-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| <span data-ttu-id="4f959-116">[обновление](../api/identitysecuritydefaultsenforcementpolicy-update.md).</span><span class="sxs-lookup"><span data-stu-id="4f959-116">[Update](../api/identitysecuritydefaultsenforcementpolicy-update.md)</span></span> | [<span data-ttu-id="4f959-117">идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="4f959-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="4f959-118">Обновление объекта **идентитисекуритидефаултсенфорцементполици** .</span><span class="sxs-lookup"><span data-stu-id="4f959-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f959-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f959-119">Properties</span></span>

| <span data-ttu-id="4f959-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f959-120">Property</span></span>     | <span data-ttu-id="4f959-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4f959-121">Type</span></span>        | <span data-ttu-id="4f959-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4f959-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f959-123">description</span><span class="sxs-lookup"><span data-stu-id="4f959-123">description</span></span>|<span data-ttu-id="4f959-124">String</span><span class="sxs-lookup"><span data-stu-id="4f959-124">String</span></span>|<span data-ttu-id="4f959-125">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f959-125">Description for this policy.</span></span> <span data-ttu-id="4f959-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f959-126">Read-only.</span></span>|
|<span data-ttu-id="4f959-127">displayName</span><span class="sxs-lookup"><span data-stu-id="4f959-127">displayName</span></span>|<span data-ttu-id="4f959-128">String</span><span class="sxs-lookup"><span data-stu-id="4f959-128">String</span></span>|<span data-ttu-id="4f959-129">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f959-129">Display name for this policy.</span></span> <span data-ttu-id="4f959-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f959-130">Read-only.</span></span>|
|<span data-ttu-id="4f959-131">id</span><span class="sxs-lookup"><span data-stu-id="4f959-131">id</span></span>|<span data-ttu-id="4f959-132">String</span><span class="sxs-lookup"><span data-stu-id="4f959-132">String</span></span>|<span data-ttu-id="4f959-133">Идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f959-133">Identifier for this policy.</span></span> <span data-ttu-id="4f959-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f959-134">Read-only.</span></span>|
|<span data-ttu-id="4f959-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4f959-135">isEnabled</span></span>|<span data-ttu-id="4f959-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f959-136">Boolean</span></span>|<span data-ttu-id="4f959-137">Если задано значение true, по умолчанию для клиента будет включен параметр безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4f959-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f959-138">Связи</span><span class="sxs-lookup"><span data-stu-id="4f959-138">Relationships</span></span>

<span data-ttu-id="4f959-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f959-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f959-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4f959-140">JSON representation</span></span>

<span data-ttu-id="4f959-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f959-141">The following is a JSON representation of the resource.</span></span>

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