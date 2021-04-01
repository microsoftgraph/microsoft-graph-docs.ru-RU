---
title: Тип ресурса identityProviderBase
description: Представляет поставщиков удостоверений в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 1a3d26697c26b803bcbac9141d7ff011575f91f7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491209"
---
# <a name="identityproviderbase-resource-type"></a><span data-ttu-id="f49b7-103">Тип ресурса identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="f49b7-103">identityProviderBase resource type</span></span>
<span data-ttu-id="f49b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f49b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f49b7-105">Представляет поставщиков удостоверений с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory и клиента Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="f49b7-105">Represents identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="f49b7-106">Для сценариев Azure AD B2B в каталоге Azure AD поставщиком удостоверений может быть [socialIdentityProvider](../resources/socialidentityprovider.md) или [builtinIdentityProvider](../resources/builtinidentityprovider.md), наследуемый от типа ресурса identityProviderBase.</span><span class="sxs-lookup"><span data-stu-id="f49b7-106">For Azure AD B2B scenarios in an Azure AD directory, the identity provider can be a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md), which will inherit from identityProviderBase resource type.</span></span>

<span data-ttu-id="f49b7-107">Настройка поставщика удостоверений в каталоге Azure AD позволяет применять новые гостевые сценарии Azure AD B2B.</span><span class="sxs-lookup"><span data-stu-id="f49b7-107">Configuring an identity provider in your Azure AD directory enables new Azure AD B2B guest scenarios.</span></span> <span data-ttu-id="f49b7-108">Например, в организации есть ресурсы в Microsoft 365, которыми нужно поделиться с пользователем Gmail.</span><span class="sxs-lookup"><span data-stu-id="f49b7-108">For example, an organization has resources in Microsoft 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="f49b7-109">Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="f49b7-109">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

<span data-ttu-id="f49b7-110">В каталоге Azure AD B2C типом поставщика удостоверений может быть [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [appleIdentityProvider](../resources/appleidentityprovider.md), наследуемый от типа ресурса identityProviderBase.</span><span class="sxs-lookup"><span data-stu-id="f49b7-110">In an Azure AD B2C directory, the identity provider type can be a [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or [appleIdentityProvider](../resources/appleidentityprovider.md), which will inherit from identityProviderBase resource type.</span></span>

<span data-ttu-id="f49b7-111">Настройка поставщика удостоверений в каталоге Azure AD B2C позволяет пользователям регистрироваться и входить в приложение с помощью учетных записей социальных сетей или настраиваемого поставщика, поддерживающего OpenID Connect.</span><span class="sxs-lookup"><span data-stu-id="f49b7-111">Configuring an identity provider in your Azure AD B2C directory enables users to sign up and sign in using a social account or a custom OpenID Connect supported provider in an application.</span></span> <span data-ttu-id="f49b7-112">Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook или собственного поставщика удостоверений, соответствующего протоколу OIDC.</span><span class="sxs-lookup"><span data-stu-id="f49b7-112">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account or their own custom identity provider that complies with OIDC protocol.</span></span>

## <a name="methods"></a><span data-ttu-id="f49b7-113">Методы</span><span class="sxs-lookup"><span data-stu-id="f49b7-113">Methods</span></span>

| <span data-ttu-id="f49b7-114">Метод</span><span class="sxs-lookup"><span data-stu-id="f49b7-114">Method</span></span>       | <span data-ttu-id="f49b7-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f49b7-115">Return Type</span></span>  |<span data-ttu-id="f49b7-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f49b7-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f49b7-117">Список</span><span class="sxs-lookup"><span data-stu-id="f49b7-117">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="f49b7-118">Коллекция identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="f49b7-118">identityProviderBase collection</span></span>|<span data-ttu-id="f49b7-119">Получение всех поставщиков удостоверений, настроенных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f49b7-119">Retrieve all identity providers configured in a tenant.</span></span>|
|[<span data-ttu-id="f49b7-120">Перечисление доступных типов поставщиков</span><span class="sxs-lookup"><span data-stu-id="f49b7-120">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="f49b7-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f49b7-121">String collection</span></span>|<span data-ttu-id="f49b7-122">Получение всех типов поставщиков удостоверений, доступных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f49b7-122">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="f49b7-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="f49b7-123">Properties</span></span>

|<span data-ttu-id="f49b7-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="f49b7-124">Property</span></span>|<span data-ttu-id="f49b7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="f49b7-125">Type</span></span>|<span data-ttu-id="f49b7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f49b7-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f49b7-127">id</span><span class="sxs-lookup"><span data-stu-id="f49b7-127">id</span></span>|<span data-ttu-id="f49b7-128">String</span><span class="sxs-lookup"><span data-stu-id="f49b7-128">String</span></span>|<span data-ttu-id="f49b7-129">Идентификатор поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="f49b7-129">The identifier of the identity provider.</span></span>|
|<span data-ttu-id="f49b7-130">displayName</span><span class="sxs-lookup"><span data-stu-id="f49b7-130">displayName</span></span>|<span data-ttu-id="f49b7-131">String</span><span class="sxs-lookup"><span data-stu-id="f49b7-131">String</span></span>|<span data-ttu-id="f49b7-132">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="f49b7-132">The display name of the identity provider.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f49b7-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f49b7-133">JSON representation</span></span>

<span data-ttu-id="f49b7-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f49b7-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String",
}
```
