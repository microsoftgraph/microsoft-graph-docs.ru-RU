---
title: Обновление identityProvider
description: Обновление свойств identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 985a6d4c80187decd5770eca150f501786222a1c
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491120"
---
# <a name="update-identityprovider"></a><span data-ttu-id="d45f4-103">Обновление identityProvider</span><span class="sxs-lookup"><span data-stu-id="d45f4-103">Update identityProvider</span></span>
<span data-ttu-id="d45f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d45f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d45f4-105">Обновление свойств объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d45f4-105">Update the properties of a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD.</span></span>

<span data-ttu-id="d45f4-106">В Azure AD B2C обновим свойства [объекта socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="d45f4-106">For Azure AD B2C, update the properties  of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d45f4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d45f4-107">Permissions</span></span>

<span data-ttu-id="d45f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d45f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d45f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d45f4-110">Permission type</span></span>      | <span data-ttu-id="d45f4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d45f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d45f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d45f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d45f4-113">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d45f4-113">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="d45f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d45f4-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d45f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d45f4-115">Not supported.</span></span>|
|<span data-ttu-id="d45f4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d45f4-116">Application</span></span>| <span data-ttu-id="d45f4-117">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d45f4-117">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="d45f4-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d45f4-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d45f4-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d45f4-119">Global Administrator</span></span>
* <span data-ttu-id="d45f4-120">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="d45f4-120">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d45f4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d45f4-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d45f4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d45f4-122">Request headers</span></span>

|<span data-ttu-id="d45f4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d45f4-123">Name</span></span>|<span data-ttu-id="d45f4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d45f4-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d45f4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d45f4-125">Authorization</span></span>|<span data-ttu-id="d45f4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d45f4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d45f4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d45f4-128">Content-Type</span></span>|<span data-ttu-id="d45f4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d45f4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d45f4-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d45f4-131">Request body</span></span>

<span data-ttu-id="d45f4-132">В теле запроса укажи объект JSON одним или более свойствами, которые необходимо обновить для объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d45f4-132">In the request body, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md) object in Azure AD tenant.</span></span>

<span data-ttu-id="d45f4-133">В Azure AD B2C предоставить объекту JSON одно или несколько свойств, которые необходимо обновить для [socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="d45f4-133">In Azure AD B2C, provide a JSON object with one or more properties that need to be updated for a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object.</span></span>

### <a name="socialidentityprovider-object"></a><span data-ttu-id="d45f4-134">объект socialIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="d45f4-134">socialIdentityProvider object</span></span>

|<span data-ttu-id="d45f4-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="d45f4-135">Property</span></span>|<span data-ttu-id="d45f4-136">Тип</span><span class="sxs-lookup"><span data-stu-id="d45f4-136">Type</span></span>|<span data-ttu-id="d45f4-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d45f4-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d45f4-138">clientId</span><span class="sxs-lookup"><span data-stu-id="d45f4-138">clientId</span></span>|<span data-ttu-id="d45f4-139">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-139">String</span></span>|<span data-ttu-id="d45f4-140">Идентификатор клиента для приложения, полученного при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-140">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="d45f4-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="d45f4-141">clientSecret</span></span>|<span data-ttu-id="d45f4-142">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-142">String</span></span>|<span data-ttu-id="d45f4-143">Секрет клиента для приложения, полученного при регистрации приложения у поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-143">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="d45f4-144">Только для записи.</span><span class="sxs-lookup"><span data-stu-id="d45f4-144">This is write-only.</span></span> <span data-ttu-id="d45f4-145">Операция чтения возвращается \* \* \* \* ".</span><span class="sxs-lookup"><span data-stu-id="d45f4-145">A read operation returns "\*\*\*\*".</span></span>|
|<span data-ttu-id="d45f4-146">displayName</span><span class="sxs-lookup"><span data-stu-id="d45f4-146">displayName</span></span>|<span data-ttu-id="d45f4-147">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-147">String</span></span>|<span data-ttu-id="d45f4-148">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-148">The display name of the identity provider.</span></span>|

### <a name="openidconnectidentityprovider-object"></a><span data-ttu-id="d45f4-149">объект openIdConnectIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="d45f4-149">openIdConnectIdentityProvider object</span></span>

|<span data-ttu-id="d45f4-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="d45f4-150">Property</span></span>|<span data-ttu-id="d45f4-151">Тип</span><span class="sxs-lookup"><span data-stu-id="d45f4-151">Type</span></span>|<span data-ttu-id="d45f4-152">Описание</span><span class="sxs-lookup"><span data-stu-id="d45f4-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d45f4-153">clientId</span><span class="sxs-lookup"><span data-stu-id="d45f4-153">clientId</span></span>|<span data-ttu-id="d45f4-154">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-154">String</span></span>|<span data-ttu-id="d45f4-155">Идентификатор клиента для приложения, полученного при регистрации приложения с поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-155">The client identifier for the application obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="d45f4-156">clientSecret</span><span class="sxs-lookup"><span data-stu-id="d45f4-156">clientSecret</span></span>|<span data-ttu-id="d45f4-157">Строка</span><span class="sxs-lookup"><span data-stu-id="d45f4-157">String</span></span>|<span data-ttu-id="d45f4-158">Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-158">The client secret for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="d45f4-159">ClientSecret имеет зависимость от **responseType**.</span><span class="sxs-lookup"><span data-stu-id="d45f4-159">The clientSecret has a dependency on **responseType**.</span></span> <ul><li><span data-ttu-id="d45f4-160">Когда **responseType** — это секрет, необходимый `code` для обмена кодами auth.</span><span class="sxs-lookup"><span data-stu-id="d45f4-160">When **responseType** is `code`, a secret is required for the auth code exchange.</span></span></li><li><span data-ttu-id="d45f4-161">Когда **responseType** `id_token` является секретом, не требуется, так как не существует обмена кодом.</span><span class="sxs-lookup"><span data-stu-id="d45f4-161">When **responseType** is `id_token` the secret is not required because there is no code exchange.</span></span> <span data-ttu-id="d45f4-162">Ответ id_token возвращается непосредственно из ответа авторизации.</span><span class="sxs-lookup"><span data-stu-id="d45f4-162">The id_token is returned directly from the authorization response.</span></span></li></ul>|
|<span data-ttu-id="d45f4-163">displayName</span><span class="sxs-lookup"><span data-stu-id="d45f4-163">displayName</span></span>|<span data-ttu-id="d45f4-164">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-164">String</span></span>|<span data-ttu-id="d45f4-165">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-165">The display name of the identity provider.</span></span>|
|<span data-ttu-id="d45f4-166">domainHint</span><span class="sxs-lookup"><span data-stu-id="d45f4-166">domainHint</span></span>|<span data-ttu-id="d45f4-167">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-167">String</span></span>|<span data-ttu-id="d45f4-168">Подсказку домена можно использовать для перехода непосредственно на вход на страницу указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-168">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="d45f4-169">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="d45f4-169">claimsMapping</span></span>|[<span data-ttu-id="d45f4-170">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="d45f4-170">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="d45f4-171">После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует.</span><span class="sxs-lookup"><span data-stu-id="d45f4-171">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="d45f4-172">Этот сложный тип захватывает это сопоставление.</span><span class="sxs-lookup"><span data-stu-id="d45f4-172">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="d45f4-173">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="d45f4-173">metadataUrl</span></span>|<span data-ttu-id="d45f4-174">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-174">String</span></span>|<span data-ttu-id="d45f4-175">URL-адрес документа метаданных поставщика удостоверений OpenID Connect.</span><span class="sxs-lookup"><span data-stu-id="d45f4-175">The URL for the metadata document of the OpenID Connect identity provider.</span></span> <span data-ttu-id="d45f4-176">Каждый поставщик удостоверений OpenID Connect описывает документ метаданных, содержащий большую часть сведений, необходимых для выполнения входных данных.</span><span class="sxs-lookup"><span data-stu-id="d45f4-176">Every OpenID Connect identity provider describes a metadata document that contains most of the information required to perform sign-in.</span></span> <span data-ttu-id="d45f4-177">К ним относятся такие сведения, как URL-адреса для использования и расположение общедоступных ключей подписи службы.</span><span class="sxs-lookup"><span data-stu-id="d45f4-177">This includes information such as the URLs to use and the location of the service's public signing keys.</span></span> <span data-ttu-id="d45f4-178">Документ метаданных OpenID Connect всегда расположен в конечной точке, в которую заканчивается `.well-known/openid-configuration` .</span><span class="sxs-lookup"><span data-stu-id="d45f4-178">The OpenID Connect metadata document is always located at an endpoint that ends in `.well-known/openid-configuration`.</span></span> <span data-ttu-id="d45f4-179">Укажет URL-адрес метаданных для поставщика удостоверений OpenID Connect, который вы добавляете.</span><span class="sxs-lookup"><span data-stu-id="d45f4-179">Provide the metadata URL for the OpenID Connect identity provider you add.</span></span>|
|<span data-ttu-id="d45f4-180">responseMode</span><span class="sxs-lookup"><span data-stu-id="d45f4-180">responseMode</span></span>|<span data-ttu-id="d45f4-181">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-181">String</span></span>|<span data-ttu-id="d45f4-182">Режим ответа определяет метод, используемый для отправки данных из пользовательского поставщика удостоверений в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="d45f4-182">The response mode defines the method used to send data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="d45f4-183">Возможные значения: `form_post` , `query` .</span><span class="sxs-lookup"><span data-stu-id="d45f4-183">Possible values: `form_post`, `query`.</span></span>|
|<span data-ttu-id="d45f4-184">responseType</span><span class="sxs-lookup"><span data-stu-id="d45f4-184">responseType</span></span>|<span data-ttu-id="d45f4-185">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-185">String</span></span>|<span data-ttu-id="d45f4-186">Тип ответа описывает тип сведений, отосланных во время первоначального вызова authorization_endpoint поставщика пользовательских удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-186">The response type describes the type of information sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="d45f4-187">Возможные значения: `code` `id_token` , `token` .</span><span class="sxs-lookup"><span data-stu-id="d45f4-187">Possible values: `code` , `id_token` , `token`.</span></span>|
|<span data-ttu-id="d45f4-188">scope</span><span class="sxs-lookup"><span data-stu-id="d45f4-188">scope</span></span>|<span data-ttu-id="d45f4-189">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-189">String</span></span>|<span data-ttu-id="d45f4-190">Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-190">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

### <a name="applemanagedidentityprovider-object"></a><span data-ttu-id="d45f4-191">объект appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="d45f4-191">appleManagedIdentityProvider object</span></span>

|<span data-ttu-id="d45f4-192">Свойство</span><span class="sxs-lookup"><span data-stu-id="d45f4-192">Property</span></span>|<span data-ttu-id="d45f4-193">Тип</span><span class="sxs-lookup"><span data-stu-id="d45f4-193">Type</span></span>|<span data-ttu-id="d45f4-194">Описание</span><span class="sxs-lookup"><span data-stu-id="d45f4-194">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d45f4-195">displayName</span><span class="sxs-lookup"><span data-stu-id="d45f4-195">displayName</span></span>|<span data-ttu-id="d45f4-196">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-196">String</span></span>|<span data-ttu-id="d45f4-197">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d45f4-197">The display name of the identity provider.</span></span>|
|<span data-ttu-id="d45f4-198">developerId</span><span class="sxs-lookup"><span data-stu-id="d45f4-198">developerId</span></span>|<span data-ttu-id="d45f4-199">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-199">String</span></span>|<span data-ttu-id="d45f4-200">Идентификатор разработчика Apple.</span><span class="sxs-lookup"><span data-stu-id="d45f4-200">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="d45f4-201">serviceId</span><span class="sxs-lookup"><span data-stu-id="d45f4-201">serviceId</span></span>|<span data-ttu-id="d45f4-202">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-202">String</span></span>|<span data-ttu-id="d45f4-203">Идентификатор разработчика Apple.</span><span class="sxs-lookup"><span data-stu-id="d45f4-203">The Apple Developer identifier.</span></span>|
|<span data-ttu-id="d45f4-204">keyId</span><span class="sxs-lookup"><span data-stu-id="d45f4-204">keyId</span></span>|<span data-ttu-id="d45f4-205">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-205">String</span></span>|<span data-ttu-id="d45f4-206">Идентификатор Ключа Apple.</span><span class="sxs-lookup"><span data-stu-id="d45f4-206">The Apple Key identifier.</span></span>|
|<span data-ttu-id="d45f4-207">certificateData</span><span class="sxs-lookup"><span data-stu-id="d45f4-207">certificateData</span></span>|<span data-ttu-id="d45f4-208">String</span><span class="sxs-lookup"><span data-stu-id="d45f4-208">String</span></span>|<span data-ttu-id="d45f4-209">Данные сертификата, которые является длинной строкой текста из сертификата, могут быть null.</span><span class="sxs-lookup"><span data-stu-id="d45f4-209">The certificate data which is a long string of text from the certificate, can be null.</span></span>|

## <a name="response"></a><span data-ttu-id="d45f4-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="d45f4-210">Response</span></span>

<span data-ttu-id="d45f4-211">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d45f4-211">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="d45f4-212">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="d45f4-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="d45f4-213">Примеры</span><span class="sxs-lookup"><span data-stu-id="d45f4-213">Examples</span></span>

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a><span data-ttu-id="d45f4-214">Пример 1. Обновление определенного **поставщика социальных удостоверений** (Azure AD или Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="d45f4-214">Example 1: Update a specific **social identity provider** (Azure AD or Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="d45f4-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="d45f4-215">Request</span></span>

<span data-ttu-id="d45f4-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d45f4-216">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```

---

#### <a name="response"></a><span data-ttu-id="d45f4-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="d45f4-217">Response</span></span>

<span data-ttu-id="d45f4-218">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d45f4-218">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="d45f4-219">Пример 2. Обновление определенного **поставщика удостоверений OpenID Connect** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="d45f4-219">Example 2: Update a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="d45f4-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="d45f4-220">Request</span></span>

<span data-ttu-id="d45f4-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d45f4-221">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```

---

#### <a name="response"></a><span data-ttu-id="d45f4-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="d45f4-222">Response</span></span>

<span data-ttu-id="d45f4-223">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d45f4-223">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-a-specific-apple-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="d45f4-224">Пример 3. Обновление определенного **поставщика удостоверений Apple** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="d45f4-224">Example 3: Update a specific **Apple identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="d45f4-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="d45f4-225">Request</span></span>

<span data-ttu-id="d45f4-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d45f4-226">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json
Content-length: 41

{
  "displayName": "Apple"
}
```

---

#### <a name="response"></a><span data-ttu-id="d45f4-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="d45f4-227">Response</span></span>

<span data-ttu-id="d45f4-228">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d45f4-228">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
