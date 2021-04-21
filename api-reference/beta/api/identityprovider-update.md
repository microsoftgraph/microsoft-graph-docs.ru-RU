---
title: Обновление identityProvider
description: Обновление свойств identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: eb441c036fd4d555a7991c30a986258300282c35
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921569"
---
# <a name="update-identityprovider-deprecated"></a><span data-ttu-id="861ea-103">Обновление identityProvider (неподготовленное)</span><span class="sxs-lookup"><span data-stu-id="861ea-103">Update identityProvider (deprecated)</span></span>

<span data-ttu-id="861ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="861ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="861ea-105">Обновление свойств объекта [identityProvider.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="861ea-105">Update the properties of an [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="861ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="861ea-106">Permissions</span></span>

<span data-ttu-id="861ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="861ea-109">Permission type</span></span>      | <span data-ttu-id="861ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="861ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="861ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="861ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="861ea-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861ea-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="861ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="861ea-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="861ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="861ea-114">Not supported.</span></span>|
|<span data-ttu-id="861ea-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="861ea-115">Application</span></span>| <span data-ttu-id="861ea-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861ea-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="861ea-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="861ea-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="861ea-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="861ea-118">Global Administrator</span></span>
* <span data-ttu-id="861ea-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="861ea-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="861ea-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="861ea-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="861ea-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="861ea-121">Request headers</span></span>

|<span data-ttu-id="861ea-122">Имя</span><span class="sxs-lookup"><span data-stu-id="861ea-122">Name</span></span>|<span data-ttu-id="861ea-123">Описание</span><span class="sxs-lookup"><span data-stu-id="861ea-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="861ea-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="861ea-124">Authorization</span></span>|<span data-ttu-id="861ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="861ea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="861ea-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="861ea-127">Content-Type</span></span>|<span data-ttu-id="861ea-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="861ea-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="861ea-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="861ea-130">Request body</span></span>

<span data-ttu-id="861ea-131">В теле запроса укажи объект JSON одним или более свойствами, которые необходимо обновить для объекта [identityProvider](../resources/identityprovider.md) или [openIdConnectProvider](../resources/openidconnectprovider.md) (только для объекта Azure AD B2C).</span><span class="sxs-lookup"><span data-stu-id="861ea-131">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="861ea-132">объект identityProvider</span><span class="sxs-lookup"><span data-stu-id="861ea-132">identityProvider object</span></span>

|<span data-ttu-id="861ea-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="861ea-133">Property</span></span>|<span data-ttu-id="861ea-134">Тип</span><span class="sxs-lookup"><span data-stu-id="861ea-134">Type</span></span>|<span data-ttu-id="861ea-135">Описание</span><span class="sxs-lookup"><span data-stu-id="861ea-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="861ea-136">clientId</span><span class="sxs-lookup"><span data-stu-id="861ea-136">clientId</span></span>|<span data-ttu-id="861ea-137">String</span><span class="sxs-lookup"><span data-stu-id="861ea-137">String</span></span>|<span data-ttu-id="861ea-138">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="861ea-138">The client ID for the application.</span></span> <span data-ttu-id="861ea-139">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-139">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="861ea-140">clientSecret</span><span class="sxs-lookup"><span data-stu-id="861ea-140">clientSecret</span></span>|<span data-ttu-id="861ea-141">String</span><span class="sxs-lookup"><span data-stu-id="861ea-141">String</span></span>|<span data-ttu-id="861ea-142">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="861ea-142">The client secret for the application.</span></span> <span data-ttu-id="861ea-143">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-143">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="861ea-144">name</span><span class="sxs-lookup"><span data-stu-id="861ea-144">name</span></span>|<span data-ttu-id="861ea-145">String</span><span class="sxs-lookup"><span data-stu-id="861ea-145">String</span></span>|<span data-ttu-id="861ea-146">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-146">The display name of the identity provider.</span></span>|
|<span data-ttu-id="861ea-147">type</span><span class="sxs-lookup"><span data-stu-id="861ea-147">type</span></span>|<span data-ttu-id="861ea-148">String</span><span class="sxs-lookup"><span data-stu-id="861ea-148">String</span></span>|<span data-ttu-id="861ea-149">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="861ea-149">The identity provider type.</span></span><ul><span data-ttu-id="861ea-150">Для сценария B2B:</span><span class="sxs-lookup"><span data-stu-id="861ea-150">For B2B scenario:</span></span><li/><span data-ttu-id="861ea-151">Google</span><span class="sxs-lookup"><span data-stu-id="861ea-151">Google</span></span><li/><span data-ttu-id="861ea-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="861ea-152">Facebook</span></span></ul><ul><span data-ttu-id="861ea-153">Для сценария B2C:</span><span class="sxs-lookup"><span data-stu-id="861ea-153">For B2C scenario:</span></span><li/><span data-ttu-id="861ea-154">Майкрософт</span><span class="sxs-lookup"><span data-stu-id="861ea-154">Microsoft</span></span><li/><span data-ttu-id="861ea-155">Google</span><span class="sxs-lookup"><span data-stu-id="861ea-155">Google</span></span><li/><span data-ttu-id="861ea-156">Amazon</span><span class="sxs-lookup"><span data-stu-id="861ea-156">Amazon</span></span><li/><span data-ttu-id="861ea-157">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="861ea-157">LinkedIn</span></span><li/><span data-ttu-id="861ea-158">Facebook</span><span class="sxs-lookup"><span data-stu-id="861ea-158">Facebook</span></span><li/><span data-ttu-id="861ea-159">GitHub</span><span class="sxs-lookup"><span data-stu-id="861ea-159">GitHub</span></span><li/><span data-ttu-id="861ea-160">Twitter</span><span class="sxs-lookup"><span data-stu-id="861ea-160">Twitter</span></span><li/><span data-ttu-id="861ea-161">Weibo</span><span class="sxs-lookup"><span data-stu-id="861ea-161">Weibo</span></span><li/><span data-ttu-id="861ea-162">QQ</span><span class="sxs-lookup"><span data-stu-id="861ea-162">QQ</span></span><li/><span data-ttu-id="861ea-163">WeChat</span><span class="sxs-lookup"><span data-stu-id="861ea-163">WeChat</span></span><li/><span data-ttu-id="861ea-164">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="861ea-164">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="861ea-165">объект openIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="861ea-165">openIdConnectProvider object</span></span>

|<span data-ttu-id="861ea-166">Свойство</span><span class="sxs-lookup"><span data-stu-id="861ea-166">Property</span></span>|<span data-ttu-id="861ea-167">Тип</span><span class="sxs-lookup"><span data-stu-id="861ea-167">Type</span></span>|<span data-ttu-id="861ea-168">Описание</span><span class="sxs-lookup"><span data-stu-id="861ea-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="861ea-169">clientId</span><span class="sxs-lookup"><span data-stu-id="861ea-169">clientId</span></span>|<span data-ttu-id="861ea-170">String</span><span class="sxs-lookup"><span data-stu-id="861ea-170">String</span></span>|<span data-ttu-id="861ea-171">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="861ea-171">The client ID for the application.</span></span> <span data-ttu-id="861ea-172">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-172">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="861ea-173">clientSecret</span><span class="sxs-lookup"><span data-stu-id="861ea-173">clientSecret</span></span>|<span data-ttu-id="861ea-174">String</span><span class="sxs-lookup"><span data-stu-id="861ea-174">String</span></span>|<span data-ttu-id="861ea-175">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="861ea-175">The client secret for the application.</span></span> <span data-ttu-id="861ea-176">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-176">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="861ea-177">name</span><span class="sxs-lookup"><span data-stu-id="861ea-177">name</span></span>|<span data-ttu-id="861ea-178">String</span><span class="sxs-lookup"><span data-stu-id="861ea-178">String</span></span>|<span data-ttu-id="861ea-179">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-179">The display name of the identity provider.</span></span>|
|<span data-ttu-id="861ea-180">type</span><span class="sxs-lookup"><span data-stu-id="861ea-180">type</span></span>|<span data-ttu-id="861ea-181">String</span><span class="sxs-lookup"><span data-stu-id="861ea-181">String</span></span>|<span data-ttu-id="861ea-182">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="861ea-182">The identity provider type.</span></span> <span data-ttu-id="861ea-183">Значение должно быть `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="861ea-183">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="861ea-184">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="861ea-184">claimsMapping</span></span>|[<span data-ttu-id="861ea-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="861ea-185">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="861ea-186">После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует.</span><span class="sxs-lookup"><span data-stu-id="861ea-186">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="861ea-187">Этот сложный тип захватывает это сопоставление.</span><span class="sxs-lookup"><span data-stu-id="861ea-187">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="861ea-188">domainHint</span><span class="sxs-lookup"><span data-stu-id="861ea-188">domainHint</span></span>|<span data-ttu-id="861ea-189">Строка</span><span class="sxs-lookup"><span data-stu-id="861ea-189">String</span></span>|<span data-ttu-id="861ea-190">Подсказку домена можно использовать для перехода непосредственно на вход на страницу указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-190">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="861ea-191">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="861ea-191">metadataUrl</span></span>|<span data-ttu-id="861ea-192">Строка</span><span class="sxs-lookup"><span data-stu-id="861ea-192">String</span></span>|<span data-ttu-id="861ea-193">URL-адрес документа метаданных поставщика удостоверений Open Id Connect.</span><span class="sxs-lookup"><span data-stu-id="861ea-193">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="861ea-194">responseMode</span><span class="sxs-lookup"><span data-stu-id="861ea-194">responseMode</span></span>|<span data-ttu-id="861ea-195">Строка</span><span class="sxs-lookup"><span data-stu-id="861ea-195">String</span></span>|<span data-ttu-id="861ea-196">Определяет метод, который следует использовать для отправки данных от поставщика пользовательских удостоверений в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="861ea-196">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="861ea-197">Можно использовать следующие режимы ответа:</span><span class="sxs-lookup"><span data-stu-id="861ea-197">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="861ea-198">`form_post` . Этот режим ответа рекомендуется для лучшей безопасности.</span><span class="sxs-lookup"><span data-stu-id="861ea-198">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="861ea-199">Ответ передается методом HTTP POST, код или маркер кодируются в теле с помощью формата application/x-www-form-urlencoded.</span><span class="sxs-lookup"><span data-stu-id="861ea-199">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="861ea-200">`query` Код или маркер возвращаются в качестве параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="861ea-200">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="861ea-201">responseType</span><span class="sxs-lookup"><span data-stu-id="861ea-201">responseType</span></span>|<span data-ttu-id="861ea-202">Строка</span><span class="sxs-lookup"><span data-stu-id="861ea-202">String</span></span>|<span data-ttu-id="861ea-203">Описывает, какие сведения отправляются в исходном вызове в authorization_endpoint поставщика пользовательских удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-203">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="861ea-204">Можно использовать следующие типы ответов:</span><span class="sxs-lookup"><span data-stu-id="861ea-204">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="861ea-205">`code` . В результате потока кода авторизации код возвращается обратно в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="861ea-205">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="861ea-206">Azure AD B2C продолжает вызывать token_endpoint, чтобы обменять код на маркер.</span><span class="sxs-lookup"><span data-stu-id="861ea-206">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="861ea-207">`id_token` . Маркер ID возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-207">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="861ea-208">`token` . Маркер доступа возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-208">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="861ea-209">(На данный момент это значение не поддерживается Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="861ea-209">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="861ea-210">scope</span><span class="sxs-lookup"><span data-stu-id="861ea-210">scope</span></span>|<span data-ttu-id="861ea-211">String</span><span class="sxs-lookup"><span data-stu-id="861ea-211">String</span></span>|<span data-ttu-id="861ea-212">Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="861ea-212">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="861ea-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="861ea-213">Response</span></span>

<span data-ttu-id="861ea-214">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="861ea-214">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="861ea-215">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="861ea-215">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="861ea-216">Примеры</span><span class="sxs-lookup"><span data-stu-id="861ea-216">Examples</span></span>

### <a name="example-1-update-a-specific-identityprovider"></a><span data-ttu-id="861ea-217">Пример 1. Обновление определенного **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="861ea-217">Example 1: Update a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="861ea-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="861ea-218">Request</span></span>

<span data-ttu-id="861ea-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="861ea-219">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```

# <a name="java"></a>[<span data-ttu-id="861ea-220">Java</span><span class="sxs-lookup"><span data-stu-id="861ea-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="861ea-221">C#</span><span class="sxs-lookup"><span data-stu-id="861ea-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="861ea-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="861ea-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="861ea-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="861ea-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="861ea-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="861ea-224">Response</span></span>

<span data-ttu-id="861ea-225">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="861ea-225">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="861ea-226">Пример 2. Обновление определенного **openIDConnectProvider** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="861ea-226">Example 2: Update a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="861ea-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="861ea-227">Request</span></span>

<span data-ttu-id="861ea-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="861ea-228">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```

# <a name="java"></a>[<span data-ttu-id="861ea-229">Java</span><span class="sxs-lookup"><span data-stu-id="861ea-229">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openidconnectprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="861ea-230">C#</span><span class="sxs-lookup"><span data-stu-id="861ea-230">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="861ea-231">JavaScript</span><span class="sxs-lookup"><span data-stu-id="861ea-231">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="861ea-232">Objective-C</span><span class="sxs-lookup"><span data-stu-id="861ea-232">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="861ea-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="861ea-233">Response</span></span>

<span data-ttu-id="861ea-234">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="861ea-234">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
