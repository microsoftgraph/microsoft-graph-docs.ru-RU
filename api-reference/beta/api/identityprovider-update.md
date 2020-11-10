---
title: Обновление identityProvider
description: Обновление свойств объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 504f151e82003a6783f26c94fda5b916eb57d25c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953360"
---
# <a name="update-identityprovider"></a><span data-ttu-id="6f2ec-103">Обновление identityProvider</span><span class="sxs-lookup"><span data-stu-id="6f2ec-103">Update identityProvider</span></span>

<span data-ttu-id="6f2ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f2ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f2ec-105">Обновление свойств объекта [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="6f2ec-105">Update the properties of an [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f2ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f2ec-106">Permissions</span></span>

<span data-ttu-id="6f2ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f2ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f2ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f2ec-109">Permission type</span></span>      | <span data-ttu-id="6f2ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f2ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f2ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f2ec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f2ec-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f2ec-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="6f2ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f2ec-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6f2ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-114">Not supported.</span></span>|
|<span data-ttu-id="6f2ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f2ec-115">Application</span></span>| <span data-ttu-id="6f2ec-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f2ec-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="6f2ec-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="6f2ec-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="6f2ec-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6f2ec-118">Global administrator</span></span>
* <span data-ttu-id="6f2ec-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="6f2ec-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="6f2ec-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f2ec-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6f2ec-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f2ec-121">Request headers</span></span>

|<span data-ttu-id="6f2ec-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6f2ec-122">Name</span></span>|<span data-ttu-id="6f2ec-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2ec-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6f2ec-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f2ec-124">Authorization</span></span>|<span data-ttu-id="6f2ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6f2ec-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f2ec-127">Content-Type</span></span>|<span data-ttu-id="6f2ec-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f2ec-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f2ec-130">Request body</span></span>

<span data-ttu-id="6f2ec-131">В тексте запроса укажите объект JSON с одним или несколькими свойствами, которые необходимо обновить для объекта [identityProvider](../resources/identityprovider.md) или [опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C).</span><span class="sxs-lookup"><span data-stu-id="6f2ec-131">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="6f2ec-132">Объект identityProvider</span><span class="sxs-lookup"><span data-stu-id="6f2ec-132">identityProvider object</span></span>

|<span data-ttu-id="6f2ec-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f2ec-133">Property</span></span>|<span data-ttu-id="6f2ec-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6f2ec-134">Type</span></span>|<span data-ttu-id="6f2ec-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2ec-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f2ec-136">clientId</span><span class="sxs-lookup"><span data-stu-id="6f2ec-136">clientId</span></span>|<span data-ttu-id="6f2ec-137">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-137">String</span></span>|<span data-ttu-id="6f2ec-138">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-138">The client ID for the application.</span></span> <span data-ttu-id="6f2ec-139">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-139">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="6f2ec-140">clientSecret</span><span class="sxs-lookup"><span data-stu-id="6f2ec-140">clientSecret</span></span>|<span data-ttu-id="6f2ec-141">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-141">String</span></span>|<span data-ttu-id="6f2ec-142">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-142">The client secret for the application.</span></span> <span data-ttu-id="6f2ec-143">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-143">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="6f2ec-144">name</span><span class="sxs-lookup"><span data-stu-id="6f2ec-144">name</span></span>|<span data-ttu-id="6f2ec-145">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-145">String</span></span>|<span data-ttu-id="6f2ec-146">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-146">The display name of the identity provider.</span></span>|
|<span data-ttu-id="6f2ec-147">type</span><span class="sxs-lookup"><span data-stu-id="6f2ec-147">type</span></span>|<span data-ttu-id="6f2ec-148">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-148">String</span></span>|<span data-ttu-id="6f2ec-149">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="6f2ec-149">The identity provider type.</span></span><ul><span data-ttu-id="6f2ec-150">Для сценария B2B:</span><span class="sxs-lookup"><span data-stu-id="6f2ec-150">For B2B scenario:</span></span><li/><span data-ttu-id="6f2ec-151">Google</span><span class="sxs-lookup"><span data-stu-id="6f2ec-151">Google</span></span><li/><span data-ttu-id="6f2ec-152">Facebook</span><span class="sxs-lookup"><span data-stu-id="6f2ec-152">Facebook</span></span></ul><ul><span data-ttu-id="6f2ec-153">Для сценария B2C:</span><span class="sxs-lookup"><span data-stu-id="6f2ec-153">For B2C scenario:</span></span><li/><span data-ttu-id="6f2ec-154">Майкрософт</span><span class="sxs-lookup"><span data-stu-id="6f2ec-154">Microsoft</span></span><li/><span data-ttu-id="6f2ec-155">Google</span><span class="sxs-lookup"><span data-stu-id="6f2ec-155">Google</span></span><li/><span data-ttu-id="6f2ec-156">Amazon</span><span class="sxs-lookup"><span data-stu-id="6f2ec-156">Amazon</span></span><li/><span data-ttu-id="6f2ec-157">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="6f2ec-157">LinkedIn</span></span><li/><span data-ttu-id="6f2ec-158">Facebook</span><span class="sxs-lookup"><span data-stu-id="6f2ec-158">Facebook</span></span><li/><span data-ttu-id="6f2ec-159">GitHub</span><span class="sxs-lookup"><span data-stu-id="6f2ec-159">GitHub</span></span><li/><span data-ttu-id="6f2ec-160">Twitter</span><span class="sxs-lookup"><span data-stu-id="6f2ec-160">Twitter</span></span><li/><span data-ttu-id="6f2ec-161">Weibo</span><span class="sxs-lookup"><span data-stu-id="6f2ec-161">Weibo</span></span><li/><span data-ttu-id="6f2ec-162">QQ</span><span class="sxs-lookup"><span data-stu-id="6f2ec-162">QQ</span></span><li/><span data-ttu-id="6f2ec-163">WeChat</span><span class="sxs-lookup"><span data-stu-id="6f2ec-163">WeChat</span></span><li/><span data-ttu-id="6f2ec-164">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="6f2ec-164">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="6f2ec-165">Объект Опенидконнектпровидер</span><span class="sxs-lookup"><span data-stu-id="6f2ec-165">openIdConnectProvider object</span></span>

|<span data-ttu-id="6f2ec-166">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f2ec-166">Property</span></span>|<span data-ttu-id="6f2ec-167">Тип</span><span class="sxs-lookup"><span data-stu-id="6f2ec-167">Type</span></span>|<span data-ttu-id="6f2ec-168">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2ec-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f2ec-169">clientId</span><span class="sxs-lookup"><span data-stu-id="6f2ec-169">clientId</span></span>|<span data-ttu-id="6f2ec-170">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-170">String</span></span>|<span data-ttu-id="6f2ec-171">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-171">The client ID for the application.</span></span> <span data-ttu-id="6f2ec-172">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-172">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="6f2ec-173">clientSecret</span><span class="sxs-lookup"><span data-stu-id="6f2ec-173">clientSecret</span></span>|<span data-ttu-id="6f2ec-174">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-174">String</span></span>|<span data-ttu-id="6f2ec-175">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-175">The client secret for the application.</span></span> <span data-ttu-id="6f2ec-176">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-176">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="6f2ec-177">name</span><span class="sxs-lookup"><span data-stu-id="6f2ec-177">name</span></span>|<span data-ttu-id="6f2ec-178">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-178">String</span></span>|<span data-ttu-id="6f2ec-179">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-179">The display name of the identity provider.</span></span>|
|<span data-ttu-id="6f2ec-180">type</span><span class="sxs-lookup"><span data-stu-id="6f2ec-180">type</span></span>|<span data-ttu-id="6f2ec-181">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-181">String</span></span>|<span data-ttu-id="6f2ec-182">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="6f2ec-182">The identity provider type.</span></span> <span data-ttu-id="6f2ec-183">Значение должно быть `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="6f2ec-183">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="6f2ec-184">клаимсмаппинг</span><span class="sxs-lookup"><span data-stu-id="6f2ec-184">claimsMapping</span></span>|[<span data-ttu-id="6f2ec-185">клаимсмаппинг</span><span class="sxs-lookup"><span data-stu-id="6f2ec-185">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="6f2ec-186">После того как поставщик ОИДК отправит токен ID обратно в Azure AD, Azure AD должен сопоставить утверждения из полученного маркера с утверждениями, которые служба Azure AD распознает и использует.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-186">After the OIDC provider sends an ID token back to Azure AD, Azure AD needs to be able to map the claims from the received token to the claims that Azure AD recognizes and uses.</span></span> <span data-ttu-id="6f2ec-187">Этот сложный тип захватывает это сопоставление.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-187">This complex type captures that mapping.</span></span>|
|<span data-ttu-id="6f2ec-188">domainHint</span><span class="sxs-lookup"><span data-stu-id="6f2ec-188">domainHint</span></span>|<span data-ttu-id="6f2ec-189">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-189">String</span></span>|<span data-ttu-id="6f2ec-190">Подсказка домена может быть использована для пропуска непосредственно к странице входа указанного поставщика удостоверений вместо того, чтобы пользователь выделе выбор среди доступных поставщиков удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-190">The domain hint can be used to skip directly to the sign in page of the specified identity provider, instead of having the user make a selection among the list of available identity providers.</span></span>|
|<span data-ttu-id="6f2ec-191">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="6f2ec-191">metadataUrl</span></span>|<span data-ttu-id="6f2ec-192">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-192">String</span></span>|<span data-ttu-id="6f2ec-193">URL-адрес документа метаданных поставщика удостоверений подключения Open ID.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-193">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="6f2ec-194">респонсемоде</span><span class="sxs-lookup"><span data-stu-id="6f2ec-194">responseMode</span></span>|<span data-ttu-id="6f2ec-195">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-195">String</span></span>|<span data-ttu-id="6f2ec-196">Определяет метод, который должен использоваться для отправки данных обратно от настраиваемого поставщика удостоверений в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-196">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="6f2ec-197">Можно использовать следующие режимы ответа:</span><span class="sxs-lookup"><span data-stu-id="6f2ec-197">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="6f2ec-198">`form_post` : Этот режим ответа рекомендуется для обеспечения лучшей безопасности.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-198">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="6f2ec-199">Ответ передается через HTTP-метод POST с кодом или маркером, закодированным в теле, с помощью формата Application/x-www-Form-урленкодед.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-199">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="6f2ec-200">`query` : Код или маркер возвращается в виде параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-200">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="6f2ec-201">responseType</span><span class="sxs-lookup"><span data-stu-id="6f2ec-201">responseType</span></span>|<span data-ttu-id="6f2ec-202">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-202">String</span></span>|<span data-ttu-id="6f2ec-203">Описывает тип сведений, которые отправляются обратно при первом вызове authorization_endpoint настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-203">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="6f2ec-204">Можно использовать следующие типы ответов:</span><span class="sxs-lookup"><span data-stu-id="6f2ec-204">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="6f2ec-205">`code` : В соответствии с процессом кода авторизации код вернется обратно в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-205">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="6f2ec-206">B2C Azure AD выполняет вызов token_endpoint для обмена кодом для маркера.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-206">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="6f2ec-207">`id_token` : Токен ID возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-207">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="6f2ec-208">`token` : Маркер доступа возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-208">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="6f2ec-209">(В настоящее время это значение не поддерживается в Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="6f2ec-209">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="6f2ec-210">scope</span><span class="sxs-lookup"><span data-stu-id="6f2ec-210">scope</span></span>|<span data-ttu-id="6f2ec-211">String</span><span class="sxs-lookup"><span data-stu-id="6f2ec-211">String</span></span>|<span data-ttu-id="6f2ec-212">Область определяет сведения и разрешения, которые вы собираетесь получить от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-212">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="6f2ec-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f2ec-213">Response</span></span>

<span data-ttu-id="6f2ec-214">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-214">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="6f2ec-215">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-215">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="6f2ec-216">Примеры</span><span class="sxs-lookup"><span data-stu-id="6f2ec-216">Examples</span></span>

### <a name="example-1-update-a-specific-identityprovider"></a><span data-ttu-id="6f2ec-217">Пример 1: обновление конкретной **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="6f2ec-217">Example 1: Update a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="6f2ec-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f2ec-218">Request</span></span>

<span data-ttu-id="6f2ec-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-219">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f2ec-220">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f2ec-220">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6f2ec-221">C#</span><span class="sxs-lookup"><span data-stu-id="6f2ec-221">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f2ec-222">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f2ec-222">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f2ec-223">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f2ec-223">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f2ec-224">Java</span><span class="sxs-lookup"><span data-stu-id="6f2ec-224">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f2ec-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f2ec-225">Response</span></span>

<span data-ttu-id="6f2ec-226">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-226">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-update-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="6f2ec-227">Пример 2: обновление конкретной **опенидконнектпровидер** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="6f2ec-227">Example 2: Update a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="6f2ec-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f2ec-228">Request</span></span>

<span data-ttu-id="6f2ec-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-229">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f2ec-230">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f2ec-230">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6f2ec-231">C#</span><span class="sxs-lookup"><span data-stu-id="6f2ec-231">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-openidconnectprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f2ec-232">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f2ec-232">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-openidconnectprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f2ec-233">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f2ec-233">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-openidconnectprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f2ec-234">Java</span><span class="sxs-lookup"><span data-stu-id="6f2ec-234">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-openidconnectprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f2ec-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f2ec-235">Response</span></span>

<span data-ttu-id="6f2ec-236">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f2ec-236">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```


