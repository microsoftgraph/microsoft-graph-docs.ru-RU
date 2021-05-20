---
title: Создание identityProvider
description: Создание нового объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3ec9797ea97a34d3ab6de3098ba60f52bb48770e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546240"
---
# <a name="create-identityprovider"></a><span data-ttu-id="2b7ce-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="2b7ce-103">Create identityProvider</span></span>

<span data-ttu-id="2b7ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b7ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b7ce-105">Создание нового [объекта socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-105">Create a new [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="2b7ce-106">В Azure AD B2C создайте новый [объект socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объект appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="2b7ce-106">In Azure AD B2C create a new [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b7ce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b7ce-107">Permissions</span></span>

<span data-ttu-id="2b7ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b7ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b7ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b7ce-110">Permission type</span></span>      | <span data-ttu-id="2b7ce-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b7ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b7ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b7ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b7ce-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7ce-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="2b7ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b7ce-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2b7ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-115">Not supported.</span></span>|
|<span data-ttu-id="2b7ce-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b7ce-116">Application</span></span>|<span data-ttu-id="2b7ce-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7ce-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="2b7ce-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="2b7ce-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="2b7ce-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2b7ce-119">Global Administrator</span></span>
* <span data-ttu-id="2b7ce-120">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="2b7ce-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2b7ce-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b7ce-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="2b7ce-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b7ce-122">Request headers</span></span>

|<span data-ttu-id="2b7ce-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2b7ce-123">Name</span></span>|<span data-ttu-id="2b7ce-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7ce-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="2b7ce-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b7ce-125">Authorization</span></span>|<span data-ttu-id="2b7ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2b7ce-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b7ce-128">Content-Type</span></span>|<span data-ttu-id="2b7ce-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b7ce-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b7ce-131">Request body</span></span>

<span data-ttu-id="2b7ce-132">В теле запроса укажи JSON представление [объекта socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-132">In the request body, provide a JSON representation of [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="2b7ce-133">В Azure AD B2C предоставляют JSON представление [socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="2b7ce-133">In Azure AD B2C provide a JSON representation of [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

<span data-ttu-id="2b7ce-134">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-134">All the properties listed in the following table are required.</span></span>

### <a name="socialidentityprovider-object"></a><span data-ttu-id="2b7ce-135">объект socialIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="2b7ce-135">socialIdentityProvider object</span></span>

|<span data-ttu-id="2b7ce-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b7ce-136">Property</span></span>|<span data-ttu-id="2b7ce-137">Тип</span><span class="sxs-lookup"><span data-stu-id="2b7ce-137">Type</span></span>|<span data-ttu-id="2b7ce-138">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7ce-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b7ce-139">clientId</span><span class="sxs-lookup"><span data-stu-id="2b7ce-139">clientId</span></span>|<span data-ttu-id="2b7ce-140">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-140">String</span></span>|<span data-ttu-id="2b7ce-141">Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-141">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="2b7ce-142">clientSecret</span><span class="sxs-lookup"><span data-stu-id="2b7ce-142">clientSecret</span></span>|<span data-ttu-id="2b7ce-143">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-143">String</span></span>|<span data-ttu-id="2b7ce-144">Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-144">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="2b7ce-145">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-145">This is write-only.</span></span> <span data-ttu-id="2b7ce-146">Операция чтения возвращает "\*\*\*\*".</span><span class="sxs-lookup"><span data-stu-id="2b7ce-146">A read operation returns "\*\*\*\*".</span></span>|
|<span data-ttu-id="2b7ce-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2b7ce-147">displayName</span></span>|<span data-ttu-id="2b7ce-148">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-148">String</span></span>|<span data-ttu-id="2b7ce-149">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-149">The display name of the identity provider.</span></span>|
|<span data-ttu-id="2b7ce-150">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="2b7ce-150">identityProviderType</span></span>|<span data-ttu-id="2b7ce-151">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7ce-151">String</span></span>|<span data-ttu-id="2b7ce-152">Возможные значения для сценария B2B: `Google`, `Facebook`.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-152">For a B2B scenario, possible values: `Google`, `Facebook`.</span></span> <span data-ttu-id="2b7ce-153">Возможные значения для сценария B2C: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-153">For a B2C scenario, possible values: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span></span>|

### <a name="openidconnectidentityprovider-object"></a><span data-ttu-id="2b7ce-154">объект openIdConnectIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="2b7ce-154">openIdConnectIdentityProvider object</span></span>

|<span data-ttu-id="2b7ce-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b7ce-155">Property</span></span>|<span data-ttu-id="2b7ce-156">Тип</span><span class="sxs-lookup"><span data-stu-id="2b7ce-156">Type</span></span>|<span data-ttu-id="2b7ce-157">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7ce-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b7ce-158">clientId</span><span class="sxs-lookup"><span data-stu-id="2b7ce-158">clientId</span></span>|<span data-ttu-id="2b7ce-159">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-159">String</span></span>|<span data-ttu-id="2b7ce-160">Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-160">The client ID for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="2b7ce-161">clientSecret</span><span class="sxs-lookup"><span data-stu-id="2b7ce-161">clientSecret</span></span>|<span data-ttu-id="2b7ce-162">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7ce-162">String</span></span>|<span data-ttu-id="2b7ce-163">Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-163">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="2b7ce-164">ClientSecret имеет зависимость от **responseType**.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-164">The clientSecret has a dependency on **responseType**.</span></span> <ul><li><span data-ttu-id="2b7ce-165">Когда **responseType** — это секрет, необходимый `code` для обмена кодами auth.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-165">When **responseType** is `code`, a secret is required for the auth code exchange.</span></span></li><li><span data-ttu-id="2b7ce-166">Когда **responseType** является секретом, не требуется, так как не существует обмена кодом id_token возвращается непосредственно `id_token` из ответа авторизации.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-166">When **responseType** is `id_token` the secret is not required because there is no code exchange—the id_token is returned directly from the authorization response.</span></span></li></ul>|
|<span data-ttu-id="2b7ce-167">displayName</span><span class="sxs-lookup"><span data-stu-id="2b7ce-167">displayName</span></span>|<span data-ttu-id="2b7ce-168">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-168">String</span></span>|<span data-ttu-id="2b7ce-169">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-169">The display name of the identity provider.</span></span>|
|<span data-ttu-id="2b7ce-170">domainHint</span><span class="sxs-lookup"><span data-stu-id="2b7ce-170">domainHint</span></span>|<span data-ttu-id="2b7ce-171">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-171">String</span></span>|<span data-ttu-id="2b7ce-172">Подсказку домена можно использовать для перехода непосредственно на вход на страницу указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-172">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="2b7ce-173">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="2b7ce-173">claimsMapping</span></span>|[<span data-ttu-id="2b7ce-174">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="2b7ce-174">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="2b7ce-175">После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-175">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="2b7ce-176">Этот сложный тип захватывает это сопоставление.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-176">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="2b7ce-177">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="2b7ce-177">metadataUrl</span></span>|<span data-ttu-id="2b7ce-178">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-178">String</span></span>|<span data-ttu-id="2b7ce-179">URL-адрес документа метаданных поставщика удостоверений OpenID Подключение.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-179">The URL for the metadata document of the OpenID Connect identity provider.</span></span> <span data-ttu-id="2b7ce-180">Каждый поставщик Подключение OpenID описывает документ метаданных, содержащий большую часть сведений, необходимых для выполнения входных данных.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-180">Every OpenID Connect identity provider describes a metadata document that contains most of the information required to perform sign-in.</span></span> <span data-ttu-id="2b7ce-181">К ним относятся такие сведения, как URL-адреса для использования и расположение общедоступных ключей подписи службы.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-181">This includes information such as the URLs to use and the location of the service's public signing keys.</span></span> <span data-ttu-id="2b7ce-182">Документ openID Подключение метаданных всегда находится в конечной точке, которая заканчивается `.well-known/openid-configuration` .</span><span class="sxs-lookup"><span data-stu-id="2b7ce-182">The OpenID Connect metadata document is always located at an endpoint that ends in `.well-known/openid-configuration`.</span></span> <span data-ttu-id="2b7ce-183">Указайте URL-адрес метаданных для поставщика удостоверений OpenID Подключение, который вы добавляете.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-183">Provide the metadata URL for the OpenID Connect identity provider you add.</span></span>|
|<span data-ttu-id="2b7ce-184">responseMode</span><span class="sxs-lookup"><span data-stu-id="2b7ce-184">responseMode</span></span>|<span data-ttu-id="2b7ce-185">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-185">String</span></span>|<span data-ttu-id="2b7ce-186">Режим ответа определяет метод, используемый для отправки данных из пользовательского поставщика удостоверений в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-186">The response mode defines the method used to send data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="2b7ce-187">Возможные значения: `form_post` , `query` .</span><span class="sxs-lookup"><span data-stu-id="2b7ce-187">Possible values: `form_post`, `query`.</span></span>|
|<span data-ttu-id="2b7ce-188">responseType</span><span class="sxs-lookup"><span data-stu-id="2b7ce-188">responseType</span></span>|<span data-ttu-id="2b7ce-189">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-189">String</span></span>|<span data-ttu-id="2b7ce-190">Тип ответа описывает тип сведений, отосланных во время первоначального вызова authorization_endpoint поставщика пользовательских удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-190">The response type describes the type of information sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="2b7ce-191">Возможные значения: `code` `id_token` , `token` .</span><span class="sxs-lookup"><span data-stu-id="2b7ce-191">Possible values: `code` , `id_token` , `token`.</span></span>|
|<span data-ttu-id="2b7ce-192">scope</span><span class="sxs-lookup"><span data-stu-id="2b7ce-192">scope</span></span>|<span data-ttu-id="2b7ce-193">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-193">String</span></span>|<span data-ttu-id="2b7ce-194">Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-194">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

### <a name="appleidentityprovider-object"></a><span data-ttu-id="2b7ce-195">объект appleIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="2b7ce-195">appleIdentityProvider object</span></span>

|<span data-ttu-id="2b7ce-196">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b7ce-196">Property</span></span>|<span data-ttu-id="2b7ce-197">Тип</span><span class="sxs-lookup"><span data-stu-id="2b7ce-197">Type</span></span>|<span data-ttu-id="2b7ce-198">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7ce-198">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b7ce-199">displayName</span><span class="sxs-lookup"><span data-stu-id="2b7ce-199">displayName</span></span>|<span data-ttu-id="2b7ce-200">String</span><span class="sxs-lookup"><span data-stu-id="2b7ce-200">String</span></span>|<span data-ttu-id="2b7ce-201">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-201">The display name of the identity provider.</span></span>|
|<span data-ttu-id="2b7ce-202">developerId</span><span class="sxs-lookup"><span data-stu-id="2b7ce-202">developerId</span></span>|<span data-ttu-id="2b7ce-203">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7ce-203">String</span></span>|<span data-ttu-id="2b7ce-204">Идентификатор разработчика Apple.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-204">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="2b7ce-205">serviceId</span><span class="sxs-lookup"><span data-stu-id="2b7ce-205">serviceId</span></span>|<span data-ttu-id="2b7ce-206">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7ce-206">String</span></span>|<span data-ttu-id="2b7ce-207">Идентификатор разработчика Apple.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-207">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="2b7ce-208">keyId</span><span class="sxs-lookup"><span data-stu-id="2b7ce-208">keyId</span></span>|<span data-ttu-id="2b7ce-209">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7ce-209">String</span></span>|<span data-ttu-id="2b7ce-210">Идентификатор Ключа Apple.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-210">The Apple Key identifier.</span></span>|
|<span data-ttu-id="2b7ce-211">certificateData</span><span class="sxs-lookup"><span data-stu-id="2b7ce-211">certificateData</span></span>|<span data-ttu-id="2b7ce-212">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7ce-212">String</span></span>|<span data-ttu-id="2b7ce-213">Данные сертификата, являющиеся длинной строкой текста из сертификата. Могут иметь значение NULL.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-213">The certificate data which is a long string of text from the certificate, can be null.</span></span>|

## <a name="response"></a><span data-ttu-id="2b7ce-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b7ce-214">Response</span></span>

<span data-ttu-id="2b7ce-215">В случае успешной работы этот метод возвращает код отклика и представление JSON объекта `201 Created` [socialIdentityProvider](../resources/socialidentityprovider.md) в тексте ответа для клиента Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-215">If successful, this method returns a `201 Created` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md) object in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="2b7ce-216">Для клиента Azure AD B2C этот метод возвращает код отклика и представление JSON для `201 Created` [socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider](../resources/appleidentityprovider.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-216">For an Azure AD B2C tenant, this method returns a `201 Created` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object in the response body.</span></span>

<span data-ttu-id="2b7ce-217">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-217">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="2b7ce-218">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b7ce-218">Examples</span></span>

### <a name="example-1-create-a-specific-social-identity-provider-azure-ad-and-azure-ad-b2c"></a><span data-ttu-id="2b7ce-219">Пример 1. Создание конкретного **поставщика социальных удостоверений** (Azure AD и Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="2b7ce-219">Example 1: Create a specific **social identity provider** (Azure AD and Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="2b7ce-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b7ce-220">Request</span></span>

<span data-ttu-id="2b7ce-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-221">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b7ce-222">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b7ce-222">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.socialIdentityProvider",
  "displayName": "Login with Amazon",
  "identityProviderType": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="2b7ce-223">C#</span><span class="sxs-lookup"><span data-stu-id="2b7ce-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-socialidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b7ce-224">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b7ce-224">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-socialidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b7ce-225">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b7ce-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-socialidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b7ce-226">Java</span><span class="sxs-lookup"><span data-stu-id="2b7ce-226">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-socialidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="2b7ce-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b7ce-227">Response</span></span>

<span data-ttu-id="2b7ce-228">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-228">The following is an example of the response.</span></span>

<span data-ttu-id="2b7ce-229">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-229">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "microsoft.graph.socialIdentityProvider",
    "id": "Amazon-OAUTH",
    "displayName": "Login with Amazon",
    "identityProviderType": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```

### <a name="example-2-create-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="2b7ce-230">Пример 2. Создание определенного поставщика **удостоверений Подключение OpenID** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="2b7ce-230">Example 2: Create a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="2b7ce-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b7ce-231">Request</span></span>

<span data-ttu-id="2b7ce-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-232">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b7ce-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b7ce-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_openidconnectidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
    "displayName": "Login with the Contoso identity provider",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "12345",
    "claimsMapping": {
        "userId": "myUserId",
        "givenName": "myGivenName",
        "surname": "mySurname",
        "email": "myEmail",
        "displayName": "myDisplayName"
    },
    "domainHint": "mycustomoidc",
    "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
    "responseMode": "form_post",
    "responseType": "code",
    "scope": "openid"
}

```
# <a name="c"></a>[<span data-ttu-id="2b7ce-234">C#</span><span class="sxs-lookup"><span data-stu-id="2b7ce-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b7ce-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b7ce-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b7ce-236">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b7ce-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b7ce-237">Java</span><span class="sxs-lookup"><span data-stu-id="2b7ce-237">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="2b7ce-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b7ce-238">Response</span></span>

<span data-ttu-id="2b7ce-239">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-239">The following is an example of the response.</span></span>

<span data-ttu-id="2b7ce-240">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-240">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "displayName": "Login with the Contoso identity provider",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```

### <a name="example-3-retrieves-apple-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="2b7ce-241">Пример 3. Извлечение поставщика удостоверений Apple (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="2b7ce-241">Example 3: Retrieves Apple identity provider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="2b7ce-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b7ce-242">Request</span></span>

<span data-ttu-id="2b7ce-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-243">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```

#### <a name="response"></a><span data-ttu-id="2b7ce-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b7ce-244">Response</span></span>

<span data-ttu-id="2b7ce-245">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-245">The following is an example of the response.</span></span>

<span data-ttu-id="2b7ce-246">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2b7ce-246">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "id": "Apple-Managed-OIDC",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```
