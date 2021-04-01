---
title: Тип ресурса socialIdentityProvider
description: Представляет поставщиков удостоверений социальных сетей в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 58e08852c99c97648447e7d0acf9946ea3227122
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491186"
---
# <a name="socialidentityprovider-resource-type"></a><span data-ttu-id="5e55d-103">Тип ресурса socialIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="5e55d-103">socialIdentityProvider resource type</span></span>
<span data-ttu-id="5e55d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e55d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e55d-105">Представляет поставщиков удостоверений социальных сетей с [внешними удостоверениями](/azure/active-directory/external-identities/) для клиента Azure Active Directory и клиента Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="5e55d-105">Represents social identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="5e55d-106">Этот тип наследуется от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="5e55d-106">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

<span data-ttu-id="5e55d-107">Для сценариев Azure AD B2B в клиенте Azure AD типом поставщика удостоверений может быть Google или Facebook.</span><span class="sxs-lookup"><span data-stu-id="5e55d-107">For Azure AD B2B scenarios in an Azure AD tenant, the identity provider type can be Google or Facebook.</span></span>

<span data-ttu-id="5e55d-108">Настройка поставщика удостоверений в клиенте Azure AD позволяет применять новые гостевые сценарии Azure AD B2B.</span><span class="sxs-lookup"><span data-stu-id="5e55d-108">Configuring an identity provider in your Azure AD tenant enables new Azure AD B2B guest scenarios.</span></span> <span data-ttu-id="5e55d-109">Например, в организации есть ресурсы в Microsoft 365, которыми нужно поделиться с пользователем Gmail.</span><span class="sxs-lookup"><span data-stu-id="5e55d-109">For example, an organization has resources in Microsoft 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="5e55d-110">Для проверки подлинности и доступа к документам пользователь Gmail использует данные учетной записи Google.</span><span class="sxs-lookup"><span data-stu-id="5e55d-110">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

<span data-ttu-id="5e55d-111">В клиенте Azure AD B2C типом поставщика удостоверений может быть Майкрософт, Google, Facebook, Amazon, LinkedIn или Twitter.</span><span class="sxs-lookup"><span data-stu-id="5e55d-111">In an Azure AD B2C tenant, the identity provider type can be Microsoft, Google, Facebook, Amazon, LinkedIn or Twitter.</span></span> <span data-ttu-id="5e55d-112">В предварительной версии доступны следующие поставщики удостоверений: Weibo, QQ, WeChat и GitHub.</span><span class="sxs-lookup"><span data-stu-id="5e55d-112">The following identity providers are in preview: Weibo, QQ, WeChat, and GitHub.</span></span>

<span data-ttu-id="5e55d-113">Настройка поставщика удостоверений в клиенте Azure AD B2C позволяет пользователям регистрироваться и входить в приложение с помощью поставщика, поддерживающего учетные записи социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="5e55d-113">Configuring an identity provider in your Azure AD B2C tenant enables users to sign up and sign in using a social account supported provider in an application.</span></span> <span data-ttu-id="5e55d-114">Например, приложение может использовать Azure AD B2C, чтобы разрешить пользователям регистрироваться в службе с помощью учетной записи Facebook.</span><span class="sxs-lookup"><span data-stu-id="5e55d-114">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account.</span></span>

## <a name="methods"></a><span data-ttu-id="5e55d-115">Методы</span><span class="sxs-lookup"><span data-stu-id="5e55d-115">Methods</span></span>

| <span data-ttu-id="5e55d-116">Метод</span><span class="sxs-lookup"><span data-stu-id="5e55d-116">Method</span></span>       | <span data-ttu-id="5e55d-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e55d-117">Return Type</span></span>  |<span data-ttu-id="5e55d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5e55d-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e55d-119">Список</span><span class="sxs-lookup"><span data-stu-id="5e55d-119">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="5e55d-120">Коллекция [identityProviderBase](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="5e55d-120">[identityProviderBase](../resources/identityproviderbase.md) collection</span></span>|<span data-ttu-id="5e55d-121">Получение всех поставщиков удостоверений, настроенных в клиенте, включая поставщиков удостоверений социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="5e55d-121">Retrieve all identity providers configured in a tenant including the social identity providers.</span></span>|
|[<span data-ttu-id="5e55d-122">Создание</span><span class="sxs-lookup"><span data-stu-id="5e55d-122">Create</span></span>](../api/identityproviderbase-post-identityproviders.md)|<span data-ttu-id="5e55d-123">socialidentityprovider</span><span class="sxs-lookup"><span data-stu-id="5e55d-123">socialidentityprovider</span></span> |<span data-ttu-id="5e55d-124">Создание поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5e55d-124">Create a new social identity provider.</span></span>|
|[<span data-ttu-id="5e55d-125">Получение</span><span class="sxs-lookup"><span data-stu-id="5e55d-125">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="5e55d-126">socialidentityprovider</span><span class="sxs-lookup"><span data-stu-id="5e55d-126">socialidentityprovider</span></span> |<span data-ttu-id="5e55d-127">Получение свойств поставщика удостоверений социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="5e55d-127">Retrieve properties of a social identity provider.</span></span>|
|[<span data-ttu-id="5e55d-128">Обновление</span><span class="sxs-lookup"><span data-stu-id="5e55d-128">Update</span></span>](../api/identityproviderbase-update.md)|<span data-ttu-id="5e55d-129">Нет</span><span class="sxs-lookup"><span data-stu-id="5e55d-129">None</span></span>|<span data-ttu-id="5e55d-130">Обновление поставщика удостоверений социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="5e55d-130">Update a social identity provider.</span></span>|
|[<span data-ttu-id="5e55d-131">Удаление</span><span class="sxs-lookup"><span data-stu-id="5e55d-131">Delete</span></span>](../api/identityproviderbase-delete.md)|<span data-ttu-id="5e55d-132">Нет</span><span class="sxs-lookup"><span data-stu-id="5e55d-132">None</span></span>|<span data-ttu-id="5e55d-133">Удаление поставщика удостоверений социальных сетей.</span><span class="sxs-lookup"><span data-stu-id="5e55d-133">Delete a social  identity provider.</span></span>|
|[<span data-ttu-id="5e55d-134">Перечисление доступных типов поставщиков</span><span class="sxs-lookup"><span data-stu-id="5e55d-134">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="5e55d-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5e55d-135">String collection</span></span>|<span data-ttu-id="5e55d-136">Получение всех типов поставщиков удостоверений, доступных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5e55d-136">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e55d-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e55d-137">Properties</span></span>

|<span data-ttu-id="5e55d-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e55d-138">Property</span></span>|<span data-ttu-id="5e55d-139">Тип</span><span class="sxs-lookup"><span data-stu-id="5e55d-139">Type</span></span>|<span data-ttu-id="5e55d-140">Описание</span><span class="sxs-lookup"><span data-stu-id="5e55d-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e55d-141">clientId</span><span class="sxs-lookup"><span data-stu-id="5e55d-141">clientId</span></span>|<span data-ttu-id="5e55d-142">String</span><span class="sxs-lookup"><span data-stu-id="5e55d-142">String</span></span>|<span data-ttu-id="5e55d-143">Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5e55d-143">The client identifier for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="5e55d-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5e55d-144">Required.</span></span>|
|<span data-ttu-id="5e55d-145">clientSecret</span><span class="sxs-lookup"><span data-stu-id="5e55d-145">clientSecret</span></span>|<span data-ttu-id="5e55d-146">String</span><span class="sxs-lookup"><span data-stu-id="5e55d-146">String</span></span>|<span data-ttu-id="5e55d-147">Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5e55d-147">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="5e55d-148">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="5e55d-148">This is write-only.</span></span> <span data-ttu-id="5e55d-149">Операция чтения возвращает "\*\*\*\*".</span><span class="sxs-lookup"><span data-stu-id="5e55d-149">A read operation returns "\*\*\*\*".</span></span> <span data-ttu-id="5e55d-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e55d-150">Required.</span></span>|
|<span data-ttu-id="5e55d-151">id</span><span class="sxs-lookup"><span data-stu-id="5e55d-151">id</span></span>|<span data-ttu-id="5e55d-152">String</span><span class="sxs-lookup"><span data-stu-id="5e55d-152">String</span></span>|<span data-ttu-id="5e55d-153">Идентификатор поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5e55d-153">The identifier of the identity provider.</span></span> <span data-ttu-id="5e55d-154">Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="5e55d-154">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="5e55d-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e55d-155">Read-only.</span></span>|
|<span data-ttu-id="5e55d-156">displayName</span><span class="sxs-lookup"><span data-stu-id="5e55d-156">displayName</span></span>|<span data-ttu-id="5e55d-157">String</span><span class="sxs-lookup"><span data-stu-id="5e55d-157">String</span></span>|<span data-ttu-id="5e55d-158">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5e55d-158">The display name of the identity provider.</span></span> <span data-ttu-id="5e55d-159">Унаследовано от [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="5e55d-159">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|
|<span data-ttu-id="5e55d-160">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="5e55d-160">identityProviderType</span></span>|<span data-ttu-id="5e55d-161">Строка</span><span class="sxs-lookup"><span data-stu-id="5e55d-161">String</span></span>|<span data-ttu-id="5e55d-162">Возможные значения для сценария B2B: `Google`, `Facebook`.</span><span class="sxs-lookup"><span data-stu-id="5e55d-162">For a B2B scenario, possible values: `Google`, `Facebook`.</span></span> <span data-ttu-id="5e55d-163">Возможные значения для сценария B2C: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span><span class="sxs-lookup"><span data-stu-id="5e55d-163">For a B2C scenario, possible values: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span></span> <span data-ttu-id="5e55d-164">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5e55d-164">Required.</span></span>|

### <a name="where-to-get-the-client-identifier-and-secret"></a><span data-ttu-id="5e55d-165">Где взять идентификатор и секрет клиента</span><span class="sxs-lookup"><span data-stu-id="5e55d-165">Where to get the client identifier and secret</span></span>

<span data-ttu-id="5e55d-166">Для каждого поставщика удостоверений существует процесс создания регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="5e55d-166">Each identity provider has a process for creating an app registration.</span></span> <span data-ttu-id="5e55d-167">Например, пользователи создают регистрацию приложения с помощью Facebook на сайте [developers.facebook.com](https://developers.facebook.com/).</span><span class="sxs-lookup"><span data-stu-id="5e55d-167">For example, users create an app registration with Facebook at [developers.facebook.com](https://developers.facebook.com/).</span></span> <span data-ttu-id="5e55d-168">Итоговый идентификатор и секрет клиента можно передать для [создания identityProvider](../api/identityproviderbase-post-identityproviders.md).</span><span class="sxs-lookup"><span data-stu-id="5e55d-168">The resulting client identifier and client secret can be passed to [create identityProvider](../api/identityproviderbase-post-identityproviders.md).</span></span> <span data-ttu-id="5e55d-169">После этого каждый объект пользователя в каталоге можно объединить с любым поставщиком удостоверений клиента для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5e55d-169">Then, each user object in the directory can be federated to any of the tenant's identity providers for authentication.</span></span> <span data-ttu-id="5e55d-170">Это позволяет пользователям входить путем ввода учетных данных на странице входа поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="5e55d-170">This enables the user to sign in by entering credentials on the identity provider's sign-in page.</span></span> <span data-ttu-id="5e55d-171">Маркер от поставщика удостоверений проверяется с помощью Azure AD перед выпуском клиентом маркера для приложения.</span><span class="sxs-lookup"><span data-stu-id="5e55d-171">The token from the identity provider is validated by Azure AD before the tenant issues a token to the application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e55d-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e55d-172">JSON representation</span></span>

<span data-ttu-id="5e55d-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e55d-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "socialIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
