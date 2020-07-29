---
title: Обновление identityProvider
description: Обновление свойств объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6bd2944211312c1b5440390f7a1c7a84de205e9f
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509702"
---
# <a name="update-identityprovider"></a><span data-ttu-id="a435d-103">Обновление identityProvider</span><span class="sxs-lookup"><span data-stu-id="a435d-103">Update identityProvider</span></span>

<span data-ttu-id="a435d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a435d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a435d-105">Обновление свойств объекта [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="a435d-105">Update the properties of an [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a435d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a435d-106">Permissions</span></span>

<span data-ttu-id="a435d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a435d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a435d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a435d-109">Permission type</span></span>      | <span data-ttu-id="a435d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a435d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a435d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a435d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a435d-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a435d-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="a435d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a435d-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="a435d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a435d-114">Not supported.</span></span>|
|<span data-ttu-id="a435d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a435d-115">Application</span></span>| <span data-ttu-id="a435d-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a435d-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="a435d-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="a435d-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="a435d-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a435d-118">Global administrator</span></span>
* <span data-ttu-id="a435d-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="a435d-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a435d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a435d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a435d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a435d-121">Request headers</span></span>

|<span data-ttu-id="a435d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a435d-122">Name</span></span>|<span data-ttu-id="a435d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a435d-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="a435d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a435d-124">Authorization</span></span>|<span data-ttu-id="a435d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a435d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a435d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a435d-127">Content-Type</span></span>|<span data-ttu-id="a435d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a435d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a435d-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a435d-130">Request body</span></span>

<span data-ttu-id="a435d-131">В тексте запроса укажите объект JSON с одним или несколькими свойствами, которые необходимо обновить для объекта [identityProvider](../resources/identityprovider.md) или [опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C).</span><span class="sxs-lookup"><span data-stu-id="a435d-131">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="a435d-132">Объект identityProvider</span><span class="sxs-lookup"><span data-stu-id="a435d-132">identityProvider object</span></span>

|<span data-ttu-id="a435d-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a435d-133">Property</span></span>|<span data-ttu-id="a435d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a435d-134">Type</span></span>|<span data-ttu-id="a435d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a435d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a435d-136">clientId</span><span class="sxs-lookup"><span data-stu-id="a435d-136">clientId</span></span>|<span data-ttu-id="a435d-137">String</span><span class="sxs-lookup"><span data-stu-id="a435d-137">String</span></span>|<span data-ttu-id="a435d-138">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="a435d-138">The client ID for the application.</span></span> <span data-ttu-id="a435d-139">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-139">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="a435d-140">clientSecret</span><span class="sxs-lookup"><span data-stu-id="a435d-140">clientSecret</span></span>|<span data-ttu-id="a435d-141">String</span><span class="sxs-lookup"><span data-stu-id="a435d-141">String</span></span>|<span data-ttu-id="a435d-142">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="a435d-142">The client secret for the application.</span></span> <span data-ttu-id="a435d-143">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-143">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="a435d-144">name</span><span class="sxs-lookup"><span data-stu-id="a435d-144">name</span></span>|<span data-ttu-id="a435d-145">String</span><span class="sxs-lookup"><span data-stu-id="a435d-145">String</span></span>|<span data-ttu-id="a435d-146">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-146">The display name of the identity provider.</span></span>|
|<span data-ttu-id="a435d-147">type</span><span class="sxs-lookup"><span data-stu-id="a435d-147">type</span></span>|<span data-ttu-id="a435d-148">String</span><span class="sxs-lookup"><span data-stu-id="a435d-148">String</span></span>|<span data-ttu-id="a435d-149">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="a435d-149">The identity provider type.</span></span><ul><span data-ttu-id="a435d-150">Для сценария B2B:</span><span class="sxs-lookup"><span data-stu-id="a435d-150">For B2B scenario:</span></span><li/><span data-ttu-id="a435d-151">Google</span><span class="sxs-lookup"><span data-stu-id="a435d-151">Google</span></span><li/><span data-ttu-id="a435d-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="a435d-152">Facebook</span></span></ul><ul><span data-ttu-id="a435d-153">Для сценария B2C:</span><span class="sxs-lookup"><span data-stu-id="a435d-153">For B2C scenario:</span></span><li/><span data-ttu-id="a435d-154">Microsoft</span><span class="sxs-lookup"><span data-stu-id="a435d-154">Microsoft</span></span><li/><span data-ttu-id="a435d-155">Google</span><span class="sxs-lookup"><span data-stu-id="a435d-155">Google</span></span><li/><span data-ttu-id="a435d-156">Amazon</span><span class="sxs-lookup"><span data-stu-id="a435d-156">Amazon</span></span><li/><span data-ttu-id="a435d-157">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="a435d-157">LinkedIn</span></span><li/><span data-ttu-id="a435d-158">Facebook</span><span class="sxs-lookup"><span data-stu-id="a435d-158">Facebook</span></span><li/><span data-ttu-id="a435d-159">GitHub</span><span class="sxs-lookup"><span data-stu-id="a435d-159">GitHub</span></span><li/><span data-ttu-id="a435d-160">Twitter</span><span class="sxs-lookup"><span data-stu-id="a435d-160">Twitter</span></span><li/><span data-ttu-id="a435d-161">Weibo</span><span class="sxs-lookup"><span data-stu-id="a435d-161">Weibo</span></span><li/><span data-ttu-id="a435d-162">QQ</span><span class="sxs-lookup"><span data-stu-id="a435d-162">QQ</span></span><li/><span data-ttu-id="a435d-163">WeChat</span><span class="sxs-lookup"><span data-stu-id="a435d-163">WeChat</span></span><li/><span data-ttu-id="a435d-164">опенидконнект</span><span class="sxs-lookup"><span data-stu-id="a435d-164">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="a435d-165">Объект Опенидконнектпровидер</span><span class="sxs-lookup"><span data-stu-id="a435d-165">openIdConnectProvider object</span></span>

|<span data-ttu-id="a435d-166">Свойство</span><span class="sxs-lookup"><span data-stu-id="a435d-166">Property</span></span>|<span data-ttu-id="a435d-167">Тип</span><span class="sxs-lookup"><span data-stu-id="a435d-167">Type</span></span>|<span data-ttu-id="a435d-168">Описание</span><span class="sxs-lookup"><span data-stu-id="a435d-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a435d-169">clientId</span><span class="sxs-lookup"><span data-stu-id="a435d-169">clientId</span></span>|<span data-ttu-id="a435d-170">String</span><span class="sxs-lookup"><span data-stu-id="a435d-170">String</span></span>|<span data-ttu-id="a435d-171">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="a435d-171">The client ID for the application.</span></span> <span data-ttu-id="a435d-172">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-172">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="a435d-173">clientSecret</span><span class="sxs-lookup"><span data-stu-id="a435d-173">clientSecret</span></span>|<span data-ttu-id="a435d-174">String</span><span class="sxs-lookup"><span data-stu-id="a435d-174">String</span></span>|<span data-ttu-id="a435d-175">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="a435d-175">The client secret for the application.</span></span> <span data-ttu-id="a435d-176">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-176">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="a435d-177">name</span><span class="sxs-lookup"><span data-stu-id="a435d-177">name</span></span>|<span data-ttu-id="a435d-178">String</span><span class="sxs-lookup"><span data-stu-id="a435d-178">String</span></span>|<span data-ttu-id="a435d-179">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-179">The display name of the identity provider.</span></span>|
|<span data-ttu-id="a435d-180">type</span><span class="sxs-lookup"><span data-stu-id="a435d-180">type</span></span>|<span data-ttu-id="a435d-181">String</span><span class="sxs-lookup"><span data-stu-id="a435d-181">String</span></span>|<span data-ttu-id="a435d-182">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="a435d-182">The identity provider type.</span></span> <span data-ttu-id="a435d-183">Значение должно быть `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="a435d-183">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="a435d-184">клаимсмаппинг</span><span class="sxs-lookup"><span data-stu-id="a435d-184">claimsMapping</span></span>|[<span data-ttu-id="a435d-185">клаимсмаппинг</span><span class="sxs-lookup"><span data-stu-id="a435d-185">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="a435d-186">После того как поставщик ОИДК отправит токен ID обратно в Azure AD, Azure AD должен сопоставить утверждения из полученного маркера с утверждениями, которые служба Azure AD распознает и использует.</span><span class="sxs-lookup"><span data-stu-id="a435d-186">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="a435d-187">Этот сложный тип захватывает это сопоставление.</span><span class="sxs-lookup"><span data-stu-id="a435d-187">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="a435d-188">domainHint</span><span class="sxs-lookup"><span data-stu-id="a435d-188">domainHint</span></span>|<span data-ttu-id="a435d-189">Строка</span><span class="sxs-lookup"><span data-stu-id="a435d-189">String</span></span>|<span data-ttu-id="a435d-190">Подсказка домена может быть использована для пропуска непосредственно к странице входа указанного поставщика удостоверений вместо того, чтобы пользователь выделе выбор среди доступных поставщиков удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-190">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="a435d-191">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="a435d-191">metadataUrl</span></span>|<span data-ttu-id="a435d-192">Строка</span><span class="sxs-lookup"><span data-stu-id="a435d-192">String</span></span>|<span data-ttu-id="a435d-193">URL-адрес документа метаданных поставщика удостоверений подключения Open ID.</span><span class="sxs-lookup"><span data-stu-id="a435d-193">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="a435d-194">респонсемоде</span><span class="sxs-lookup"><span data-stu-id="a435d-194">responseMode</span></span>|<span data-ttu-id="a435d-195">Строка</span><span class="sxs-lookup"><span data-stu-id="a435d-195">String</span></span>|<span data-ttu-id="a435d-196">Определяет метод, который должен использоваться для отправки данных обратно от настраиваемого поставщика удостоверений в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="a435d-196">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="a435d-197">Можно использовать следующие режимы ответа:</span><span class="sxs-lookup"><span data-stu-id="a435d-197">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="a435d-198">`form_post`: Этот режим ответа рекомендуется для обеспечения лучшей безопасности.</span><span class="sxs-lookup"><span data-stu-id="a435d-198">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="a435d-199">Ответ передается через HTTP-метод POST с кодом или маркером, закодированным в теле, с помощью формата Application/x-www-Form-урленкодед.</span><span class="sxs-lookup"><span data-stu-id="a435d-199">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="a435d-200">`query`: Код или маркер возвращается в виде параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="a435d-200">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="a435d-201">responseType</span><span class="sxs-lookup"><span data-stu-id="a435d-201">responseType</span></span>|<span data-ttu-id="a435d-202">Строка</span><span class="sxs-lookup"><span data-stu-id="a435d-202">String</span></span>|<span data-ttu-id="a435d-203">Описывает тип сведений, которые отправляются обратно при первом вызове authorization_endpoint настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-203">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="a435d-204">Можно использовать следующие типы ответов:</span><span class="sxs-lookup"><span data-stu-id="a435d-204">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="a435d-205">`code`: В соответствии с процессом кода авторизации код вернется обратно в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="a435d-205">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="a435d-206">B2C Azure AD выполняет вызов token_endpoint для обмена кодом для маркера.</span><span class="sxs-lookup"><span data-stu-id="a435d-206">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="a435d-207">`id_token`: Токен ID возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-207">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="a435d-208">`token`: Маркер доступа возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-208">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="a435d-209">(В настоящее время это значение не поддерживается в Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="a435d-209">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="a435d-210">scope</span><span class="sxs-lookup"><span data-stu-id="a435d-210">scope</span></span>|<span data-ttu-id="a435d-211">Строка</span><span class="sxs-lookup"><span data-stu-id="a435d-211">String</span></span>|<span data-ttu-id="a435d-212">Область определяет сведения и разрешения, которые вы собираетесь получить от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a435d-212">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="a435d-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="a435d-213">Response</span></span>

<span data-ttu-id="a435d-214">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a435d-214">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="a435d-215">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="a435d-215">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="a435d-216">Примеры</span><span class="sxs-lookup"><span data-stu-id="a435d-216">Examples</span></span>

### <a name="example-1-update-a-specific-identityprovider"></a><span data-ttu-id="a435d-217">Пример 1: обновление конкретной **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="a435d-217">Example 1: Update a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="a435d-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="a435d-218">Request</span></span>

<span data-ttu-id="a435d-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a435d-219">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a435d-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="a435d-220">Response</span></span>

<span data-ttu-id="a435d-221">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a435d-221">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-update-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="a435d-222">Пример 2: обновление конкретной **опенидконнектпровидер** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="a435d-222">Example 2: Update a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="a435d-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="a435d-223">Request</span></span>

<span data-ttu-id="a435d-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a435d-224">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a435d-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="a435d-225">Response</span></span>

<span data-ttu-id="a435d-226">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a435d-226">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
