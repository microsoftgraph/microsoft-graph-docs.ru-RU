---
title: Тип ресурса builtInIdentityProvider
description: Представляет встроенных поставщиков удостоверений в клиенте Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 5c806306e596a087a6c4006dc39b1804c130858a
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491197"
---
# <a name="builtinidentityprovider-resource-type"></a><span data-ttu-id="70032-103">Тип ресурса builtInIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="70032-103">builtInIdentityProvider resource type</span></span>
<span data-ttu-id="70032-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70032-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70032-105">Представляет встроенных поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70032-105">Represents built-in identity providers with [External Identities](/azure/active-directory/external-identities/) for an Azure Active Directory tenant.</span></span>

<span data-ttu-id="70032-106">Для сценариев Azure AD B2B в клиенте Azure AD встроенным типом поставщика удостоверений может быть Azure Active Directory (AAD), учетная запись Майкрософт (MSA) или одноразовый секретный код по почте (EmailOTP).</span><span class="sxs-lookup"><span data-stu-id="70032-106">For Azure AD B2B scenarios in an Azure AD tenant, the built in identity provider type can be an Azure Active Directory(AAD), Microsoft account(MSA) or email one-time passcode (EmailOTP).</span></span>

<span data-ttu-id="70032-107">Этот тип наследуется от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="70032-107">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="70032-108">Методы</span><span class="sxs-lookup"><span data-stu-id="70032-108">Methods</span></span>

| <span data-ttu-id="70032-109">Метод</span><span class="sxs-lookup"><span data-stu-id="70032-109">Method</span></span>       | <span data-ttu-id="70032-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="70032-110">Return Type</span></span>  |<span data-ttu-id="70032-111">Описание</span><span class="sxs-lookup"><span data-stu-id="70032-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70032-112">Список</span><span class="sxs-lookup"><span data-stu-id="70032-112">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="70032-113">Коллекция [identityProviderBase](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="70032-113">[identityProviderBase](../resources/identityproviderbase.md) collection</span></span>|<span data-ttu-id="70032-114">Получение всех поставщиков удостоверений, настроенных в клиенте, включая встроенных поставщиков удостоверений.</span><span class="sxs-lookup"><span data-stu-id="70032-114">Retrieve all identity providers configured in a tenant including the built-in identity providers.</span></span>|
|[<span data-ttu-id="70032-115">Получение</span><span class="sxs-lookup"><span data-stu-id="70032-115">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="70032-116">builtInIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="70032-116">builtInIdentityProvider</span></span>|<span data-ttu-id="70032-117">Получение свойств встроенного поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="70032-117">Retrieve properties of an built-in identity provider.</span></span>|
|[<span data-ttu-id="70032-118">Перечисление доступных типов поставщиков</span><span class="sxs-lookup"><span data-stu-id="70032-118">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="70032-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="70032-119">String collection</span></span>|<span data-ttu-id="70032-120">Получение всех типов поставщиков удостоверений, доступных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="70032-120">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="70032-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="70032-121">Properties</span></span>

|<span data-ttu-id="70032-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="70032-122">Property</span></span>|<span data-ttu-id="70032-123">Тип</span><span class="sxs-lookup"><span data-stu-id="70032-123">Type</span></span>|<span data-ttu-id="70032-124">Описание</span><span class="sxs-lookup"><span data-stu-id="70032-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70032-125">id</span><span class="sxs-lookup"><span data-stu-id="70032-125">id</span></span>|<span data-ttu-id="70032-126">String</span><span class="sxs-lookup"><span data-stu-id="70032-126">String</span></span>|<span data-ttu-id="70032-127">Идентификатор поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="70032-127">The identifier of the identity provider.</span></span> <span data-ttu-id="70032-128">Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="70032-128">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="70032-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70032-129">Read-only.</span></span>|
|<span data-ttu-id="70032-130">displayName</span><span class="sxs-lookup"><span data-stu-id="70032-130">displayName</span></span>|<span data-ttu-id="70032-131">String</span><span class="sxs-lookup"><span data-stu-id="70032-131">String</span></span>|<span data-ttu-id="70032-132">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="70032-132">The display name of the identity provider.</span></span> <span data-ttu-id="70032-133">Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="70032-133">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|
|<span data-ttu-id="70032-134">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="70032-134">identityProviderType</span></span>|<span data-ttu-id="70032-135">String</span><span class="sxs-lookup"><span data-stu-id="70032-135">String</span></span>|<span data-ttu-id="70032-136">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="70032-136">The identity provider type.</span></span> <span data-ttu-id="70032-137">Возможные значения для сценария B2B: `AADSignup`, `MicrosoftAccount`, `EmailOTP`.</span><span class="sxs-lookup"><span data-stu-id="70032-137">For a B2B scenario, possible values: `AADSignup`, `MicrosoftAccount`, `EmailOTP`.</span></span> <span data-ttu-id="70032-138">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="70032-138">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70032-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70032-139">JSON representation</span></span>

<span data-ttu-id="70032-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70032-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "builtinIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
