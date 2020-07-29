---
title: Создание identityProvider
description: Создание нового объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5d6eb847179a062bda1c0013bafb73de38ab455
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509709"
---
# <a name="create-identityprovider"></a><span data-ttu-id="4c894-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="4c894-103">Create identityProvider</span></span>

<span data-ttu-id="4c894-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c894-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c894-105">Создание нового объекта [identityProvider](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="4c894-105">Create a new [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c894-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c894-106">Permissions</span></span>

<span data-ttu-id="4c894-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c894-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c894-109">Permission type</span></span>      | <span data-ttu-id="4c894-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c894-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c894-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c894-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c894-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c894-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="4c894-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c894-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4c894-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c894-114">Not supported.</span></span>|
|<span data-ttu-id="4c894-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c894-115">Application</span></span>|<span data-ttu-id="4c894-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c894-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="4c894-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="4c894-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="4c894-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4c894-118">Global administrator</span></span>
* <span data-ttu-id="4c894-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="4c894-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4c894-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c894-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="4c894-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c894-121">Request headers</span></span>

|<span data-ttu-id="4c894-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4c894-122">Name</span></span>|<span data-ttu-id="4c894-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4c894-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4c894-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c894-124">Authorization</span></span>|<span data-ttu-id="4c894-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c894-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4c894-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c894-127">Content-Type</span></span>|<span data-ttu-id="4c894-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c894-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c894-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c894-130">Request body</span></span>

<span data-ttu-id="4c894-131">В тексте запроса предоставьте представление объекта [identityProvider](../resources/identityprovider.md) или [опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c894-131">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span> <span data-ttu-id="4c894-132">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="4c894-132">All the properties listed in the following table are required.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="4c894-133">Объект identityProvider</span><span class="sxs-lookup"><span data-stu-id="4c894-133">identityProvider object</span></span>

|<span data-ttu-id="4c894-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c894-134">Property</span></span>|<span data-ttu-id="4c894-135">Тип</span><span class="sxs-lookup"><span data-stu-id="4c894-135">Type</span></span>|<span data-ttu-id="4c894-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4c894-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c894-137">clientId</span><span class="sxs-lookup"><span data-stu-id="4c894-137">clientId</span></span>|<span data-ttu-id="4c894-138">String</span><span class="sxs-lookup"><span data-stu-id="4c894-138">String</span></span>|<span data-ttu-id="4c894-139">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="4c894-139">The client ID for the application.</span></span> <span data-ttu-id="4c894-140">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-140">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="4c894-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="4c894-141">clientSecret</span></span>|<span data-ttu-id="4c894-142">String</span><span class="sxs-lookup"><span data-stu-id="4c894-142">String</span></span>|<span data-ttu-id="4c894-143">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="4c894-143">The client secret for the application.</span></span> <span data-ttu-id="4c894-144">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-144">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="4c894-145">name</span><span class="sxs-lookup"><span data-stu-id="4c894-145">name</span></span>|<span data-ttu-id="4c894-146">String</span><span class="sxs-lookup"><span data-stu-id="4c894-146">String</span></span>|<span data-ttu-id="4c894-147">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-147">The display name of the identity provider.</span></span>|
|<span data-ttu-id="4c894-148">type</span><span class="sxs-lookup"><span data-stu-id="4c894-148">type</span></span>|<span data-ttu-id="4c894-149">String</span><span class="sxs-lookup"><span data-stu-id="4c894-149">String</span></span>|<span data-ttu-id="4c894-150">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="4c894-150">The identity provider type.</span></span> <ul><span data-ttu-id="4c894-151">Для сценария B2B:</span><span class="sxs-lookup"><span data-stu-id="4c894-151">For B2B scenario:</span></span><li/><span data-ttu-id="4c894-152">Google</span><span class="sxs-lookup"><span data-stu-id="4c894-152">Google</span></span><li/><span data-ttu-id="4c894-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="4c894-153">Facebook</span></span></ul><ul><span data-ttu-id="4c894-154">Для сценария B2C:</span><span class="sxs-lookup"><span data-stu-id="4c894-154">For B2C scenario:</span></span><li/><span data-ttu-id="4c894-155">Microsoft</span><span class="sxs-lookup"><span data-stu-id="4c894-155">Microsoft</span></span><li/><span data-ttu-id="4c894-156">Google</span><span class="sxs-lookup"><span data-stu-id="4c894-156">Google</span></span><li/><span data-ttu-id="4c894-157">Amazon</span><span class="sxs-lookup"><span data-stu-id="4c894-157">Amazon</span></span><li/><span data-ttu-id="4c894-158">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="4c894-158">LinkedIn</span></span><li/><span data-ttu-id="4c894-159">Facebook</span><span class="sxs-lookup"><span data-stu-id="4c894-159">Facebook</span></span><li/><span data-ttu-id="4c894-160">GitHub</span><span class="sxs-lookup"><span data-stu-id="4c894-160">GitHub</span></span><li/><span data-ttu-id="4c894-161">Twitter</span><span class="sxs-lookup"><span data-stu-id="4c894-161">Twitter</span></span><li/><span data-ttu-id="4c894-162">Weibo</span><span class="sxs-lookup"><span data-stu-id="4c894-162">Weibo</span></span><li/><span data-ttu-id="4c894-163">QQ</span><span class="sxs-lookup"><span data-stu-id="4c894-163">QQ</span></span><li/><span data-ttu-id="4c894-164">WeChat</span><span class="sxs-lookup"><span data-stu-id="4c894-164">WeChat</span></span><li/><span data-ttu-id="4c894-165">опенидконнект</span><span class="sxs-lookup"><span data-stu-id="4c894-165">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="4c894-166">Объект Опенидконнектпровидер</span><span class="sxs-lookup"><span data-stu-id="4c894-166">openIdConnectProvider object</span></span>

|<span data-ttu-id="4c894-167">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c894-167">Property</span></span>|<span data-ttu-id="4c894-168">Тип</span><span class="sxs-lookup"><span data-stu-id="4c894-168">Type</span></span>|<span data-ttu-id="4c894-169">Описание</span><span class="sxs-lookup"><span data-stu-id="4c894-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c894-170">clientId</span><span class="sxs-lookup"><span data-stu-id="4c894-170">clientId</span></span>|<span data-ttu-id="4c894-171">String</span><span class="sxs-lookup"><span data-stu-id="4c894-171">String</span></span>|<span data-ttu-id="4c894-172">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="4c894-172">The client ID for the application.</span></span> <span data-ttu-id="4c894-173">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-173">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="4c894-174">clientSecret</span><span class="sxs-lookup"><span data-stu-id="4c894-174">clientSecret</span></span>|<span data-ttu-id="4c894-175">String</span><span class="sxs-lookup"><span data-stu-id="4c894-175">String</span></span>|<span data-ttu-id="4c894-176">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="4c894-176">The client secret for the application.</span></span> <span data-ttu-id="4c894-177">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-177">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="4c894-178">name</span><span class="sxs-lookup"><span data-stu-id="4c894-178">name</span></span>|<span data-ttu-id="4c894-179">String</span><span class="sxs-lookup"><span data-stu-id="4c894-179">String</span></span>|<span data-ttu-id="4c894-180">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-180">The display name of the identity provider.</span></span>|
|<span data-ttu-id="4c894-181">type</span><span class="sxs-lookup"><span data-stu-id="4c894-181">type</span></span>|<span data-ttu-id="4c894-182">String</span><span class="sxs-lookup"><span data-stu-id="4c894-182">String</span></span>|<span data-ttu-id="4c894-183">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="4c894-183">The identity provider type.</span></span> <span data-ttu-id="4c894-184">Значение должно быть `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="4c894-184">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="4c894-185">клаимсмаппинг</span><span class="sxs-lookup"><span data-stu-id="4c894-185">claimsMapping</span></span>|[<span data-ttu-id="4c894-186">клаимсмаппинг</span><span class="sxs-lookup"><span data-stu-id="4c894-186">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="4c894-187">`userId`Свойства и `displayname` обязательные для объекта клаимсмаппинг.</span><span class="sxs-lookup"><span data-stu-id="4c894-187">The `userId` and `displayname` properties are required in the claimsMapping object.</span></span>|
|<span data-ttu-id="4c894-188">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="4c894-188">metadataUrl</span></span>|<span data-ttu-id="4c894-189">Строка</span><span class="sxs-lookup"><span data-stu-id="4c894-189">String</span></span>|<span data-ttu-id="4c894-190">URL-адрес документа метаданных поставщика удостоверений подключения Open ID.</span><span class="sxs-lookup"><span data-stu-id="4c894-190">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="4c894-191">респонсемоде</span><span class="sxs-lookup"><span data-stu-id="4c894-191">responseMode</span></span>|<span data-ttu-id="4c894-192">Строка</span><span class="sxs-lookup"><span data-stu-id="4c894-192">String</span></span>|<span data-ttu-id="4c894-193">Определяет метод, который должен использоваться для отправки данных обратно от настраиваемого поставщика удостоверений в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="4c894-193">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="4c894-194">Можно использовать следующие режимы ответа:</span><span class="sxs-lookup"><span data-stu-id="4c894-194">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="4c894-195">`form_post`: Этот режим ответа рекомендуется для обеспечения лучшей безопасности.</span><span class="sxs-lookup"><span data-stu-id="4c894-195">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="4c894-196">Ответ передается через HTTP-метод POST с кодом или маркером, закодированным в теле, с помощью формата Application/x-www-Form-урленкодед.</span><span class="sxs-lookup"><span data-stu-id="4c894-196">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="4c894-197">`query`: Код или маркер возвращается в виде параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="4c894-197">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="4c894-198">responseType</span><span class="sxs-lookup"><span data-stu-id="4c894-198">responseType</span></span>|<span data-ttu-id="4c894-199">Строка</span><span class="sxs-lookup"><span data-stu-id="4c894-199">String</span></span>|<span data-ttu-id="4c894-200">Описывает тип сведений, которые отправляются обратно при первом вызове authorization_endpoint настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-200">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="4c894-201">Можно использовать следующие типы ответов:</span><span class="sxs-lookup"><span data-stu-id="4c894-201">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="4c894-202">`code`: В соответствии с процессом кода авторизации код вернется обратно в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="4c894-202">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="4c894-203">B2C Azure AD выполняет вызов token_endpoint для обмена кодом для маркера.</span><span class="sxs-lookup"><span data-stu-id="4c894-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="4c894-204">`id_token`: Токен ID возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-204">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="4c894-205">`token`: Маркер доступа возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-205">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="4c894-206">(В настоящее время это значение не поддерживается в Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="4c894-206">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="4c894-207">scope</span><span class="sxs-lookup"><span data-stu-id="4c894-207">scope</span></span>|<span data-ttu-id="4c894-208">Строка</span><span class="sxs-lookup"><span data-stu-id="4c894-208">String</span></span>|<span data-ttu-id="4c894-209">Область определяет сведения и разрешения, которые вы собираетесь получить от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4c894-209">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="4c894-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c894-210">Response</span></span>

<span data-ttu-id="4c894-211">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и [IdentityProvider](../resources/identityprovider.md) или [Опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c894-211">If successful, this method returns a `201 Created` response code and [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object in the response body.</span></span> <span data-ttu-id="4c894-212">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="4c894-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="4c894-213">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c894-213">Examples</span></span>

### <a name="example-1-create-a-specific-identityprovider"></a><span data-ttu-id="4c894-214">Пример 1: создание определенного **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="4c894-214">Example 1: Create a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="4c894-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c894-215">Request</span></span>

<span data-ttu-id="4c894-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c894-216">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="4c894-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c894-217">Response</span></span>

<span data-ttu-id="4c894-218">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c894-218">The following is an example of the response.</span></span>

<span data-ttu-id="4c894-219">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c894-219">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="4c894-220">Пример 2: создание определенного **опенидконнектпровидер** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="4c894-220">Example 2: Create a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="4c894-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c894-221">Request</span></span>

<span data-ttu-id="4c894-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c894-222">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="4c894-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c894-223">Response</span></span>

<span data-ttu-id="4c894-224">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c894-224">The following is an example of the response.</span></span>

<span data-ttu-id="4c894-225">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c894-225">**Note:** The response object shown here might be shortened for readability.</span></span>

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
