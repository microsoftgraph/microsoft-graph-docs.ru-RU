---
title: Создание identityProvider
description: Создание нового объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 987ce00a1f3c39e148e99c8743ec669009462e2b
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566722"
---
# <a name="create-identityprovider"></a><span data-ttu-id="103f9-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="103f9-103">Create identityProvider</span></span>

<span data-ttu-id="103f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="103f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="103f9-105">Создание нового объекта [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="103f9-105">Create a new [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="103f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="103f9-106">Permissions</span></span>

<span data-ttu-id="103f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="103f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="103f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="103f9-109">Permission type</span></span>      | <span data-ttu-id="103f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="103f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="103f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="103f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="103f9-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="103f9-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="103f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="103f9-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="103f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="103f9-114">Not supported.</span></span>|
|<span data-ttu-id="103f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="103f9-115">Application</span></span>|<span data-ttu-id="103f9-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="103f9-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="103f9-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="103f9-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="103f9-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="103f9-118">Global administrator</span></span>
* <span data-ttu-id="103f9-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="103f9-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="103f9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="103f9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="103f9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="103f9-121">Request headers</span></span>

|<span data-ttu-id="103f9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="103f9-122">Name</span></span>|<span data-ttu-id="103f9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="103f9-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="103f9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="103f9-124">Authorization</span></span>|<span data-ttu-id="103f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="103f9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="103f9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="103f9-127">Content-Type</span></span>|<span data-ttu-id="103f9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="103f9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="103f9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="103f9-130">Request body</span></span>

<span data-ttu-id="103f9-131">В тексте запроса предоставьте представление объекта [identityProvider](../resources/identityprovider.md) или [опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="103f9-131">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span> <span data-ttu-id="103f9-132">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="103f9-132">All the properties listed in the following table are required.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="103f9-133">Объект identityProvider</span><span class="sxs-lookup"><span data-stu-id="103f9-133">identityProvider object</span></span>

|<span data-ttu-id="103f9-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="103f9-134">Property</span></span>|<span data-ttu-id="103f9-135">Тип</span><span class="sxs-lookup"><span data-stu-id="103f9-135">Type</span></span>|<span data-ttu-id="103f9-136">Описание</span><span class="sxs-lookup"><span data-stu-id="103f9-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="103f9-137">clientId</span><span class="sxs-lookup"><span data-stu-id="103f9-137">clientId</span></span>|<span data-ttu-id="103f9-138">String</span><span class="sxs-lookup"><span data-stu-id="103f9-138">String</span></span>|<span data-ttu-id="103f9-139">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="103f9-139">The client ID for the application.</span></span> <span data-ttu-id="103f9-140">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-140">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="103f9-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="103f9-141">clientSecret</span></span>|<span data-ttu-id="103f9-142">String</span><span class="sxs-lookup"><span data-stu-id="103f9-142">String</span></span>|<span data-ttu-id="103f9-143">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="103f9-143">The client secret for the application.</span></span> <span data-ttu-id="103f9-144">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-144">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="103f9-145">name</span><span class="sxs-lookup"><span data-stu-id="103f9-145">name</span></span>|<span data-ttu-id="103f9-146">String</span><span class="sxs-lookup"><span data-stu-id="103f9-146">String</span></span>|<span data-ttu-id="103f9-147">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-147">The display name of the identity provider.</span></span>|
|<span data-ttu-id="103f9-148">type</span><span class="sxs-lookup"><span data-stu-id="103f9-148">type</span></span>|<span data-ttu-id="103f9-149">String</span><span class="sxs-lookup"><span data-stu-id="103f9-149">String</span></span>|<span data-ttu-id="103f9-150">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="103f9-150">The identity provider type.</span></span> <ul><span data-ttu-id="103f9-151">Для сценария B2B:</span><span class="sxs-lookup"><span data-stu-id="103f9-151">For B2B scenario:</span></span><li/><span data-ttu-id="103f9-152">Google</span><span class="sxs-lookup"><span data-stu-id="103f9-152">Google</span></span><li/><span data-ttu-id="103f9-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="103f9-153">Facebook</span></span></ul><ul><span data-ttu-id="103f9-154">Для сценария B2C:</span><span class="sxs-lookup"><span data-stu-id="103f9-154">For B2C scenario:</span></span><li/><span data-ttu-id="103f9-155">Майкрософт</span><span class="sxs-lookup"><span data-stu-id="103f9-155">Microsoft</span></span><li/><span data-ttu-id="103f9-156">Google</span><span class="sxs-lookup"><span data-stu-id="103f9-156">Google</span></span><li/><span data-ttu-id="103f9-157">Amazon</span><span class="sxs-lookup"><span data-stu-id="103f9-157">Amazon</span></span><li/><span data-ttu-id="103f9-158">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="103f9-158">LinkedIn</span></span><li/><span data-ttu-id="103f9-159">Facebook</span><span class="sxs-lookup"><span data-stu-id="103f9-159">Facebook</span></span><li/><span data-ttu-id="103f9-160">GitHub</span><span class="sxs-lookup"><span data-stu-id="103f9-160">GitHub</span></span><li/><span data-ttu-id="103f9-161">Twitter</span><span class="sxs-lookup"><span data-stu-id="103f9-161">Twitter</span></span><li/><span data-ttu-id="103f9-162">Weibo</span><span class="sxs-lookup"><span data-stu-id="103f9-162">Weibo</span></span><li/><span data-ttu-id="103f9-163">QQ</span><span class="sxs-lookup"><span data-stu-id="103f9-163">QQ</span></span><li/><span data-ttu-id="103f9-164">WeChat</span><span class="sxs-lookup"><span data-stu-id="103f9-164">WeChat</span></span><li/><span data-ttu-id="103f9-165">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="103f9-165">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="103f9-166">Объект Опенидконнектпровидер</span><span class="sxs-lookup"><span data-stu-id="103f9-166">openIdConnectProvider object</span></span>

|<span data-ttu-id="103f9-167">Свойство</span><span class="sxs-lookup"><span data-stu-id="103f9-167">Property</span></span>|<span data-ttu-id="103f9-168">Тип</span><span class="sxs-lookup"><span data-stu-id="103f9-168">Type</span></span>|<span data-ttu-id="103f9-169">Описание</span><span class="sxs-lookup"><span data-stu-id="103f9-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="103f9-170">clientId</span><span class="sxs-lookup"><span data-stu-id="103f9-170">clientId</span></span>|<span data-ttu-id="103f9-171">String</span><span class="sxs-lookup"><span data-stu-id="103f9-171">String</span></span>|<span data-ttu-id="103f9-172">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="103f9-172">The client ID for the application.</span></span> <span data-ttu-id="103f9-173">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-173">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="103f9-174">clientSecret</span><span class="sxs-lookup"><span data-stu-id="103f9-174">clientSecret</span></span>|<span data-ttu-id="103f9-175">String</span><span class="sxs-lookup"><span data-stu-id="103f9-175">String</span></span>|<span data-ttu-id="103f9-176">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="103f9-176">The client secret for the application.</span></span> <span data-ttu-id="103f9-177">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-177">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="103f9-178">name</span><span class="sxs-lookup"><span data-stu-id="103f9-178">name</span></span>|<span data-ttu-id="103f9-179">String</span><span class="sxs-lookup"><span data-stu-id="103f9-179">String</span></span>|<span data-ttu-id="103f9-180">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-180">The display name of the identity provider.</span></span>|
|<span data-ttu-id="103f9-181">type</span><span class="sxs-lookup"><span data-stu-id="103f9-181">type</span></span>|<span data-ttu-id="103f9-182">String</span><span class="sxs-lookup"><span data-stu-id="103f9-182">String</span></span>|<span data-ttu-id="103f9-183">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="103f9-183">The identity provider type.</span></span> <span data-ttu-id="103f9-184">Значение должно быть `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="103f9-184">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="103f9-185">клаимсмаппинг</span><span class="sxs-lookup"><span data-stu-id="103f9-185">claimsMapping</span></span>|[<span data-ttu-id="103f9-186">клаимсмаппинг</span><span class="sxs-lookup"><span data-stu-id="103f9-186">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="103f9-187">`userId`Свойства и `displayname` обязательные для объекта клаимсмаппинг.</span><span class="sxs-lookup"><span data-stu-id="103f9-187">The `userId` and `displayname` properties are required in the claimsMapping object.</span></span>|
|<span data-ttu-id="103f9-188">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="103f9-188">metadataUrl</span></span>|<span data-ttu-id="103f9-189">String</span><span class="sxs-lookup"><span data-stu-id="103f9-189">String</span></span>|<span data-ttu-id="103f9-190">URL-адрес документа метаданных поставщика удостоверений подключения Open ID.</span><span class="sxs-lookup"><span data-stu-id="103f9-190">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="103f9-191">респонсемоде</span><span class="sxs-lookup"><span data-stu-id="103f9-191">responseMode</span></span>|<span data-ttu-id="103f9-192">String</span><span class="sxs-lookup"><span data-stu-id="103f9-192">String</span></span>|<span data-ttu-id="103f9-193">Определяет метод, который должен использоваться для отправки данных обратно от настраиваемого поставщика удостоверений в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="103f9-193">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="103f9-194">Можно использовать следующие режимы ответа:</span><span class="sxs-lookup"><span data-stu-id="103f9-194">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="103f9-195">`form_post`: Этот режим ответа рекомендуется для обеспечения лучшей безопасности.</span><span class="sxs-lookup"><span data-stu-id="103f9-195">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="103f9-196">Ответ передается через HTTP-метод POST с кодом или маркером, закодированным в теле, с помощью формата Application/x-www-Form-урленкодед.</span><span class="sxs-lookup"><span data-stu-id="103f9-196">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="103f9-197">`query`: Код или маркер возвращается в виде параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="103f9-197">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="103f9-198">responseType</span><span class="sxs-lookup"><span data-stu-id="103f9-198">responseType</span></span>|<span data-ttu-id="103f9-199">String</span><span class="sxs-lookup"><span data-stu-id="103f9-199">String</span></span>|<span data-ttu-id="103f9-200">Описывает тип сведений, которые отправляются обратно при первом вызове authorization_endpoint настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-200">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="103f9-201">Можно использовать следующие типы ответов:</span><span class="sxs-lookup"><span data-stu-id="103f9-201">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="103f9-202">`code`: В соответствии с процессом кода авторизации код вернется обратно в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="103f9-202">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="103f9-203">B2C Azure AD выполняет вызов token_endpoint для обмена кодом для маркера.</span><span class="sxs-lookup"><span data-stu-id="103f9-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="103f9-204">`id_token`: Токен ID возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-204">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="103f9-205">`token`: Маркер доступа возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-205">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="103f9-206">(В настоящее время это значение не поддерживается в Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="103f9-206">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="103f9-207">scope</span><span class="sxs-lookup"><span data-stu-id="103f9-207">scope</span></span>|<span data-ttu-id="103f9-208">Строка</span><span class="sxs-lookup"><span data-stu-id="103f9-208">String</span></span>|<span data-ttu-id="103f9-209">Область определяет сведения и разрешения, которые вы собираетесь получить от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="103f9-209">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="103f9-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="103f9-210">Response</span></span>

<span data-ttu-id="103f9-211">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и [IdentityProvider](../resources/identityprovider.md) или [Опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="103f9-211">If successful, this method returns a `201 Created` response code and [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object in the response body.</span></span> <span data-ttu-id="103f9-212">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="103f9-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="103f9-213">Примеры</span><span class="sxs-lookup"><span data-stu-id="103f9-213">Examples</span></span>

### <a name="example-1-create-a-specific-identityprovider"></a><span data-ttu-id="103f9-214">Пример 1: создание определенного **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="103f9-214">Example 1: Create a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="103f9-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="103f9-215">Request</span></span>

<span data-ttu-id="103f9-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="103f9-216">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="103f9-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="103f9-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.identityProvider",
  "name": "Login with Amazon",
  "type": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="103f9-218">C#</span><span class="sxs-lookup"><span data-stu-id="103f9-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="103f9-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="103f9-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="103f9-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="103f9-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="103f9-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="103f9-221">Response</span></span>

<span data-ttu-id="103f9-222">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="103f9-222">The following is an example of the response.</span></span>

<span data-ttu-id="103f9-223">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="103f9-223">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.type": "microsoft.graph.identityProvider",
    "id": "Amazon-OAUTH",
    "name": "Login with Amazon",
    "type": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```
### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="103f9-224">Пример 2: создание определенного **опенидконнектпровидер** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="103f9-224">Example 2: Create a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="103f9-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="103f9-225">Request</span></span>

<span data-ttu-id="103f9-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="103f9-226">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="103f9-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="103f9-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_openidconnectprovider_from_identityproviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
    "name": "Login with the Contoso identity provider",
    "type": "OpenIDConnect",
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
# <a name="c"></a>[<span data-ttu-id="103f9-228">C#</span><span class="sxs-lookup"><span data-stu-id="103f9-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="103f9-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="103f9-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="103f9-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="103f9-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="103f9-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="103f9-231">Response</span></span>

<span data-ttu-id="103f9-232">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="103f9-232">The following is an example of the response.</span></span>

<span data-ttu-id="103f9-233">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="103f9-233">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
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
