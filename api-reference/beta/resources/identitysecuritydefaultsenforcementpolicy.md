---
title: Тип ресурса Идентитисекуритидефаултсенфорцементполици
description: Представляет политику безопасности по умолчанию для Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4771af4502df2154435ae6b403fa12e3e265217a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218466"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="65843-104">Тип ресурса Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="65843-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="65843-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65843-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65843-106">Представляет политику [безопасности по умолчанию](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="65843-106">Represents the Azure Active Directory [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="65843-107">Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="65843-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="65843-108">Наследуется от [основы](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="65843-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="65843-109">Методы</span><span class="sxs-lookup"><span data-stu-id="65843-109">Methods</span></span>

| <span data-ttu-id="65843-110">Метод</span><span class="sxs-lookup"><span data-stu-id="65843-110">Method</span></span>       | <span data-ttu-id="65843-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65843-111">Return Type</span></span> | <span data-ttu-id="65843-112">Описание</span><span class="sxs-lookup"><span data-stu-id="65843-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="65843-113">[получение](../api/identitysecuritydefaultsenforcementpolicy-get.md);</span><span class="sxs-lookup"><span data-stu-id="65843-113">[Get](../api/identitysecuritydefaultsenforcementpolicy-get.md)</span></span> | [<span data-ttu-id="65843-114">идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="65843-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="65843-115">Чтение свойств объекта **идентитисекуритидефаултсенфорцементполици** .</span><span class="sxs-lookup"><span data-stu-id="65843-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| <span data-ttu-id="65843-116">[обновление](../api/identitysecuritydefaultsenforcementpolicy-update.md).</span><span class="sxs-lookup"><span data-stu-id="65843-116">[Update](../api/identitysecuritydefaultsenforcementpolicy-update.md)</span></span> | [<span data-ttu-id="65843-117">идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="65843-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="65843-118">Обновление объекта **идентитисекуритидефаултсенфорцементполици** .</span><span class="sxs-lookup"><span data-stu-id="65843-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="65843-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="65843-119">Properties</span></span>

| <span data-ttu-id="65843-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="65843-120">Property</span></span>     | <span data-ttu-id="65843-121">Тип</span><span class="sxs-lookup"><span data-stu-id="65843-121">Type</span></span>        | <span data-ttu-id="65843-122">Описание</span><span class="sxs-lookup"><span data-stu-id="65843-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65843-123">description</span><span class="sxs-lookup"><span data-stu-id="65843-123">description</span></span>|<span data-ttu-id="65843-124">String</span><span class="sxs-lookup"><span data-stu-id="65843-124">String</span></span>|<span data-ttu-id="65843-125">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="65843-125">Description for this policy.</span></span> <span data-ttu-id="65843-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65843-126">Read-only.</span></span>|
|<span data-ttu-id="65843-127">displayName</span><span class="sxs-lookup"><span data-stu-id="65843-127">displayName</span></span>|<span data-ttu-id="65843-128">Строка</span><span class="sxs-lookup"><span data-stu-id="65843-128">String</span></span>|<span data-ttu-id="65843-129">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="65843-129">Display name for this policy.</span></span> <span data-ttu-id="65843-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65843-130">Read-only.</span></span>|
|<span data-ttu-id="65843-131">id</span><span class="sxs-lookup"><span data-stu-id="65843-131">id</span></span>|<span data-ttu-id="65843-132">String</span><span class="sxs-lookup"><span data-stu-id="65843-132">String</span></span>|<span data-ttu-id="65843-133">Идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="65843-133">Identifier for this policy.</span></span> <span data-ttu-id="65843-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65843-134">Read-only.</span></span>|
|<span data-ttu-id="65843-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="65843-135">isEnabled</span></span>|<span data-ttu-id="65843-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="65843-136">Boolean</span></span>|<span data-ttu-id="65843-137">Если задано значение true, по умолчанию для клиента будет включен параметр безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="65843-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65843-138">Связи</span><span class="sxs-lookup"><span data-stu-id="65843-138">Relationships</span></span>

<span data-ttu-id="65843-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="65843-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65843-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="65843-140">JSON representation</span></span>

<span data-ttu-id="65843-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65843-141">The following is a JSON representation of the resource.</span></span>

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
