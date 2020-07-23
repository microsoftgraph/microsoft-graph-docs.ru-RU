---
title: Тип ресурса Идентитисекуритидефаултсенфорцементполици
description: Представляет политику безопасности по умолчанию для Azure Active Directory. Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e3275588e51cb48a0c72745812da0679ca971008
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384898"
---
# <a name="identitysecuritydefaultsenforcementpolicy-resource-type"></a><span data-ttu-id="0e18f-104">Тип ресурса Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="0e18f-104">identitySecurityDefaultsEnforcementPolicy resource type</span></span>

<span data-ttu-id="0e18f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e18f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e18f-106">Представляет политику [безопасности по умолчанию](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) для Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0e18f-106">Represents the Azure Active Directory [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) policy.</span></span> <span data-ttu-id="0e18f-107">Параметры безопасности по умолчанию содержат предварительно настроенные параметры безопасности, которые защищаются от распространенных атак.</span><span class="sxs-lookup"><span data-stu-id="0e18f-107">Security defaults contain preconfigured security settings that protect against common attacks.</span></span>

<span data-ttu-id="0e18f-108">Наследуется от [основы](../resources/policybase.md).</span><span class="sxs-lookup"><span data-stu-id="0e18f-108">Inherits from [policyBase](../resources/policybase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0e18f-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0e18f-109">Methods</span></span>

| <span data-ttu-id="0e18f-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0e18f-110">Method</span></span>       | <span data-ttu-id="0e18f-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0e18f-111">Return Type</span></span> | <span data-ttu-id="0e18f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0e18f-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0e18f-113">[получение](../api/identitysecuritydefaultsenforcementpolicy-get.md);</span><span class="sxs-lookup"><span data-stu-id="0e18f-113">[Get](../api/identitysecuritydefaultsenforcementpolicy-get.md)</span></span> | [<span data-ttu-id="0e18f-114">идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="0e18f-114">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="0e18f-115">Чтение свойств объекта **идентитисекуритидефаултсенфорцементполици** .</span><span class="sxs-lookup"><span data-stu-id="0e18f-115">Read the properties of an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |
| <span data-ttu-id="0e18f-116">[обновление](../api/identitysecuritydefaultsenforcementpolicy-update.md).</span><span class="sxs-lookup"><span data-stu-id="0e18f-116">[Update](../api/identitysecuritydefaultsenforcementpolicy-update.md)</span></span> | [<span data-ttu-id="0e18f-117">идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="0e18f-117">identitySecurityDefaultsEnforcementPolicy</span></span>](identitysecuritydefaultsenforcementpolicy.md) | <span data-ttu-id="0e18f-118">Обновление объекта **идентитисекуритидефаултсенфорцементполици** .</span><span class="sxs-lookup"><span data-stu-id="0e18f-118">Update an **identitySecurityDefaultsEnforcementPolicy** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0e18f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e18f-119">Properties</span></span>

| <span data-ttu-id="0e18f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e18f-120">Property</span></span>     | <span data-ttu-id="0e18f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0e18f-121">Type</span></span>        | <span data-ttu-id="0e18f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0e18f-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e18f-123">description</span><span class="sxs-lookup"><span data-stu-id="0e18f-123">description</span></span>|<span data-ttu-id="0e18f-124">String</span><span class="sxs-lookup"><span data-stu-id="0e18f-124">String</span></span>|<span data-ttu-id="0e18f-125">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e18f-125">Description for this policy.</span></span> <span data-ttu-id="0e18f-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e18f-126">Read-only.</span></span>|
|<span data-ttu-id="0e18f-127">displayName</span><span class="sxs-lookup"><span data-stu-id="0e18f-127">displayName</span></span>|<span data-ttu-id="0e18f-128">Строка</span><span class="sxs-lookup"><span data-stu-id="0e18f-128">String</span></span>|<span data-ttu-id="0e18f-129">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e18f-129">Display name for this policy.</span></span> <span data-ttu-id="0e18f-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e18f-130">Read-only.</span></span>|
|<span data-ttu-id="0e18f-131">id</span><span class="sxs-lookup"><span data-stu-id="0e18f-131">id</span></span>|<span data-ttu-id="0e18f-132">String</span><span class="sxs-lookup"><span data-stu-id="0e18f-132">String</span></span>|<span data-ttu-id="0e18f-133">Идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0e18f-133">Identifier for this policy.</span></span> <span data-ttu-id="0e18f-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e18f-134">Read-only.</span></span>|
|<span data-ttu-id="0e18f-135">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0e18f-135">isEnabled</span></span>|<span data-ttu-id="0e18f-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e18f-136">Boolean</span></span>|<span data-ttu-id="0e18f-137">Если задано значение true, по умолчанию для клиента будет включен параметр безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0e18f-137">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e18f-138">Связи</span><span class="sxs-lookup"><span data-stu-id="0e18f-138">Relationships</span></span>

<span data-ttu-id="0e18f-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0e18f-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e18f-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0e18f-140">JSON representation</span></span>

<span data-ttu-id="0e18f-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e18f-141">The following is a JSON representation of the resource.</span></span>

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
