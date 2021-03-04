---
title: Создание identityProvider
description: Создание нового объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 93a59a479adae11840f967aaa9745f20828cdce6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435457"
---
# <a name="create-identityprovider"></a><span data-ttu-id="3a0c0-103">Создание identityProvider</span><span class="sxs-lookup"><span data-stu-id="3a0c0-103">Create identityProvider</span></span>

<span data-ttu-id="3a0c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a0c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a0c0-105">Создание нового [объекта identityProvider.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="3a0c0-105">Create a new [identityProvider](../resources/identityprovider.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a0c0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a0c0-106">Permissions</span></span>

<span data-ttu-id="3a0c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a0c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a0c0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a0c0-109">Permission type</span></span>      | <span data-ttu-id="3a0c0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a0c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a0c0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a0c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a0c0-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a0c0-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="3a0c0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a0c0-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3a0c0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-114">Not supported.</span></span>|
|<span data-ttu-id="3a0c0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a0c0-115">Application</span></span>|<span data-ttu-id="3a0c0-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a0c0-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="3a0c0-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="3a0c0-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="3a0c0-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3a0c0-118">Global administrator</span></span>
* <span data-ttu-id="3a0c0-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="3a0c0-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3a0c0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a0c0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="3a0c0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a0c0-121">Request headers</span></span>

|<span data-ttu-id="3a0c0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3a0c0-122">Name</span></span>|<span data-ttu-id="3a0c0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3a0c0-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3a0c0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a0c0-124">Authorization</span></span>|<span data-ttu-id="3a0c0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3a0c0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a0c0-127">Content-Type</span></span>|<span data-ttu-id="3a0c0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a0c0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a0c0-130">Request body</span></span>

<span data-ttu-id="3a0c0-131">В теле запроса укажи JSON представление [объекта identityProvider](../resources/identityprovider.md) или [openIdConnectProvider](../resources/openidconnectprovider.md) (только для объекта Azure AD B2C).</span><span class="sxs-lookup"><span data-stu-id="3a0c0-131">In the request body, provide a JSON representation of [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object.</span></span> <span data-ttu-id="3a0c0-132">Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-132">All the properties listed in the following table are required.</span></span>

### <a name="identityprovider-object"></a><span data-ttu-id="3a0c0-133">объект identityProvider</span><span class="sxs-lookup"><span data-stu-id="3a0c0-133">identityProvider object</span></span>

|<span data-ttu-id="3a0c0-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a0c0-134">Property</span></span>|<span data-ttu-id="3a0c0-135">Тип</span><span class="sxs-lookup"><span data-stu-id="3a0c0-135">Type</span></span>|<span data-ttu-id="3a0c0-136">Описание</span><span class="sxs-lookup"><span data-stu-id="3a0c0-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a0c0-137">clientId</span><span class="sxs-lookup"><span data-stu-id="3a0c0-137">clientId</span></span>|<span data-ttu-id="3a0c0-138">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-138">String</span></span>|<span data-ttu-id="3a0c0-139">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-139">The client ID for the application.</span></span> <span data-ttu-id="3a0c0-140">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-140">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="3a0c0-141">clientSecret</span><span class="sxs-lookup"><span data-stu-id="3a0c0-141">clientSecret</span></span>|<span data-ttu-id="3a0c0-142">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-142">String</span></span>|<span data-ttu-id="3a0c0-143">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-143">The client secret for the application.</span></span> <span data-ttu-id="3a0c0-144">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-144">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="3a0c0-145">name</span><span class="sxs-lookup"><span data-stu-id="3a0c0-145">name</span></span>|<span data-ttu-id="3a0c0-146">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-146">String</span></span>|<span data-ttu-id="3a0c0-147">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-147">The display name of the identity provider.</span></span>|
|<span data-ttu-id="3a0c0-148">type</span><span class="sxs-lookup"><span data-stu-id="3a0c0-148">type</span></span>|<span data-ttu-id="3a0c0-149">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-149">String</span></span>|<span data-ttu-id="3a0c0-150">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="3a0c0-150">The identity provider type.</span></span> <ul><span data-ttu-id="3a0c0-151">Для сценария B2B:</span><span class="sxs-lookup"><span data-stu-id="3a0c0-151">For B2B scenario:</span></span><li/><span data-ttu-id="3a0c0-152">Google</span><span class="sxs-lookup"><span data-stu-id="3a0c0-152">Google</span></span><li/><span data-ttu-id="3a0c0-153">Facebook</span><span class="sxs-lookup"><span data-stu-id="3a0c0-153">Facebook</span></span></ul><ul><span data-ttu-id="3a0c0-154">Для сценария B2C:</span><span class="sxs-lookup"><span data-stu-id="3a0c0-154">For B2C scenario:</span></span><li/><span data-ttu-id="3a0c0-155">Майкрософт</span><span class="sxs-lookup"><span data-stu-id="3a0c0-155">Microsoft</span></span><li/><span data-ttu-id="3a0c0-156">Google</span><span class="sxs-lookup"><span data-stu-id="3a0c0-156">Google</span></span><li/><span data-ttu-id="3a0c0-157">Amazon</span><span class="sxs-lookup"><span data-stu-id="3a0c0-157">Amazon</span></span><li/><span data-ttu-id="3a0c0-158">LinkedIn</span><span class="sxs-lookup"><span data-stu-id="3a0c0-158">LinkedIn</span></span><li/><span data-ttu-id="3a0c0-159">Facebook</span><span class="sxs-lookup"><span data-stu-id="3a0c0-159">Facebook</span></span><li/><span data-ttu-id="3a0c0-160">GitHub</span><span class="sxs-lookup"><span data-stu-id="3a0c0-160">GitHub</span></span><li/><span data-ttu-id="3a0c0-161">Twitter</span><span class="sxs-lookup"><span data-stu-id="3a0c0-161">Twitter</span></span><li/><span data-ttu-id="3a0c0-162">Weibo</span><span class="sxs-lookup"><span data-stu-id="3a0c0-162">Weibo</span></span><li/><span data-ttu-id="3a0c0-163">QQ</span><span class="sxs-lookup"><span data-stu-id="3a0c0-163">QQ</span></span><li/><span data-ttu-id="3a0c0-164">WeChat</span><span class="sxs-lookup"><span data-stu-id="3a0c0-164">WeChat</span></span><li/><span data-ttu-id="3a0c0-165">OpenIDConnect</span><span class="sxs-lookup"><span data-stu-id="3a0c0-165">OpenIDConnect</span></span></ul>|

### <a name="openidconnectprovider-object"></a><span data-ttu-id="3a0c0-166">объект openIdConnectProvider</span><span class="sxs-lookup"><span data-stu-id="3a0c0-166">openIdConnectProvider object</span></span>

|<span data-ttu-id="3a0c0-167">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a0c0-167">Property</span></span>|<span data-ttu-id="3a0c0-168">Тип</span><span class="sxs-lookup"><span data-stu-id="3a0c0-168">Type</span></span>|<span data-ttu-id="3a0c0-169">Описание</span><span class="sxs-lookup"><span data-stu-id="3a0c0-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a0c0-170">clientId</span><span class="sxs-lookup"><span data-stu-id="3a0c0-170">clientId</span></span>|<span data-ttu-id="3a0c0-171">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-171">String</span></span>|<span data-ttu-id="3a0c0-172">Идентификатор клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-172">The client ID for the application.</span></span> <span data-ttu-id="3a0c0-173">Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-173">This is the client ID obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="3a0c0-174">clientSecret</span><span class="sxs-lookup"><span data-stu-id="3a0c0-174">clientSecret</span></span>|<span data-ttu-id="3a0c0-175">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-175">String</span></span>|<span data-ttu-id="3a0c0-176">Секрет клиента для приложения.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-176">The client secret for the application.</span></span> <span data-ttu-id="3a0c0-177">Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-177">This is the client secret obtained when registering the application with the identity provider.</span></span>|
|<span data-ttu-id="3a0c0-178">name</span><span class="sxs-lookup"><span data-stu-id="3a0c0-178">name</span></span>|<span data-ttu-id="3a0c0-179">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-179">String</span></span>|<span data-ttu-id="3a0c0-180">Отображаемое имя поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-180">The display name of the identity provider.</span></span>|
|<span data-ttu-id="3a0c0-181">type</span><span class="sxs-lookup"><span data-stu-id="3a0c0-181">type</span></span>|<span data-ttu-id="3a0c0-182">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-182">String</span></span>|<span data-ttu-id="3a0c0-183">Тип поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="3a0c0-183">The identity provider type.</span></span> <span data-ttu-id="3a0c0-184">Значение должно быть `OpenIdConnect` .</span><span class="sxs-lookup"><span data-stu-id="3a0c0-184">The value must be `OpenIdConnect`.</span></span>|
|<span data-ttu-id="3a0c0-185">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="3a0c0-185">claimsMapping</span></span>|[<span data-ttu-id="3a0c0-186">claimsMapping</span><span class="sxs-lookup"><span data-stu-id="3a0c0-186">claimsMapping</span></span>](../resources/claimsmapping.md)|<span data-ttu-id="3a0c0-187">Свойства `userId` и свойства необходимы в `displayname` объекте claimsMapping.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-187">The `userId` and `displayname` properties are required in the claimsMapping object.</span></span>|
|<span data-ttu-id="3a0c0-188">metadataUrl</span><span class="sxs-lookup"><span data-stu-id="3a0c0-188">metadataUrl</span></span>|<span data-ttu-id="3a0c0-189">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-189">String</span></span>|<span data-ttu-id="3a0c0-190">URL-адрес документа метаданных поставщика удостоверений Open Id Connect.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-190">The URL for the metadata document of the Open Id Connect identity provider.</span></span>|
|<span data-ttu-id="3a0c0-191">responseMode</span><span class="sxs-lookup"><span data-stu-id="3a0c0-191">responseMode</span></span>|<span data-ttu-id="3a0c0-192">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-192">String</span></span>|<span data-ttu-id="3a0c0-193">Определяет метод, который следует использовать для отправки данных от поставщика пользовательских удостоверений в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-193">Defines the method that should be used to send the data back from the custom identity provider to Azure AD B2C.</span></span> <span data-ttu-id="3a0c0-194">Можно использовать следующие режимы ответа:</span><span class="sxs-lookup"><span data-stu-id="3a0c0-194">The following response modes can be used:</span></span> <ul><li/><span data-ttu-id="3a0c0-195">`form_post` . Этот режим ответа рекомендуется для лучшей безопасности.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-195">`form_post` : This response mode is recommended for best security.</span></span> <span data-ttu-id="3a0c0-196">Ответ передается методом HTTP POST, код или маркер кодируются в теле с помощью формата application/x-www-form-urlencoded.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-196">The response is transmitted via the HTTP POST method, with the code or token being encoded in the body using the application/x-www-form-urlencoded format.</span></span><li/><span data-ttu-id="3a0c0-197">`query` Код или маркер возвращаются в качестве параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-197">`query` : The code or token is returned as a query parameter.</span></span></ul>|
|<span data-ttu-id="3a0c0-198">responseType</span><span class="sxs-lookup"><span data-stu-id="3a0c0-198">responseType</span></span>|<span data-ttu-id="3a0c0-199">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-199">String</span></span>|<span data-ttu-id="3a0c0-200">Описывает, какие сведения отправляются в исходном вызове в authorization_endpoint поставщика пользовательских удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-200">Describes what kind of information is sent back in the initial call to the authorization_endpoint of the custom identity provider.</span></span> <span data-ttu-id="3a0c0-201">Можно использовать следующие типы ответов:</span><span class="sxs-lookup"><span data-stu-id="3a0c0-201">The following response types can be used:</span></span><ul><li/> <span data-ttu-id="3a0c0-202">`code` . В результате потока кода авторизации код возвращается обратно в Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-202">`code` : As per the authorization code flow, a code will be returned back to Azure AD B2C.</span></span> <span data-ttu-id="3a0c0-203">Azure AD B2C продолжает вызывать token_endpoint, чтобы обменять код на маркер.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-203">Azure AD B2C proceeds to call the token_endpoint to exchange the code for the token.</span></span><li/> <span data-ttu-id="3a0c0-204">`id_token` . Маркер ID возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-204">`id_token` : An ID token is returned back to Azure AD B2C from the custom identity provider.</span></span> <li/><span data-ttu-id="3a0c0-205">`token` . Маркер доступа возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-205">`token` : An access token is returned back to Azure AD B2C from the custom identity provider.</span></span> <span data-ttu-id="3a0c0-206">(На данный момент это значение не поддерживается Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="3a0c0-206">(This value is not supported by Azure AD B2C at the moment)</span></span></ul>|
|<span data-ttu-id="3a0c0-207">scope</span><span class="sxs-lookup"><span data-stu-id="3a0c0-207">scope</span></span>|<span data-ttu-id="3a0c0-208">String</span><span class="sxs-lookup"><span data-stu-id="3a0c0-208">String</span></span>|<span data-ttu-id="3a0c0-209">Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-209">Scope defines the information and permissions you are looking to gather from your custom identity provider.</span></span>|

## <a name="response"></a><span data-ttu-id="3a0c0-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a0c0-210">Response</span></span>

<span data-ttu-id="3a0c0-211">В случае успешной работы этот метод возвращает код ответа и `201 Created` [identityProvider](../resources/identityprovider.md) или [openIdConnectProvider](../resources/openidconnectprovider.md) (только для объекта Azure AD B2C) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-211">If successful, this method returns a `201 Created` response code and [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) object in the response body.</span></span> <span data-ttu-id="3a0c0-212">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-212">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="3a0c0-213">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a0c0-213">Examples</span></span>

### <a name="example-1-create-a-specific-identityprovider"></a><span data-ttu-id="3a0c0-214">Пример 1. Создание определенного **identityProvider**</span><span class="sxs-lookup"><span data-stu-id="3a0c0-214">Example 1: Create a specific **identityProvider**</span></span>

#### <a name="request"></a><span data-ttu-id="3a0c0-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a0c0-215">Request</span></span>

<span data-ttu-id="3a0c0-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-216">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a0c0-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a0c0-217">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3a0c0-218">C#</span><span class="sxs-lookup"><span data-stu-id="3a0c0-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a0c0-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a0c0-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a0c0-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a0c0-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a0c0-221">Java</span><span class="sxs-lookup"><span data-stu-id="3a0c0-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a0c0-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a0c0-222">Response</span></span>

<span data-ttu-id="3a0c0-223">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-223">The following is an example of the response.</span></span>

<span data-ttu-id="3a0c0-224">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-224">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
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
### <a name="example-2-create-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="3a0c0-225">Пример 2. Создание определенного **openIDConnectProvider** (только для Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="3a0c0-225">Example 2: Create a specific **openIDConnectProvider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="3a0c0-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a0c0-226">Request</span></span>

<span data-ttu-id="3a0c0-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-227">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a0c0-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a0c0-228">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3a0c0-229">C#</span><span class="sxs-lookup"><span data-stu-id="3a0c0-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-openidconnectprovider-from-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a0c0-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a0c0-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-openidconnectprovider-from-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a0c0-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a0c0-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-openidconnectprovider-from-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a0c0-232">Java</span><span class="sxs-lookup"><span data-stu-id="3a0c0-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-openidconnectprovider-from-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a0c0-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a0c0-233">Response</span></span>

<span data-ttu-id="3a0c0-234">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-234">The following is an example of the response.</span></span>

<span data-ttu-id="3a0c0-235">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a0c0-235">**Note:** The response object shown here might be shortened for readability.</span></span>

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


