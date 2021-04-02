---
title: Создание b2cIdentityUserFlow
description: Создайте новый объект b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 620d6a395c87c8507a9fd6c2bb9d5742a8b560da
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508885"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="84566-103">Создание b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="84566-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="84566-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84566-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84566-105">Создайте [новый объект b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="84566-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84566-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84566-106">Permissions</span></span>

<span data-ttu-id="84566-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84566-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84566-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84566-109">Permission type</span></span>      | <span data-ttu-id="84566-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84566-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84566-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84566-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84566-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84566-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="84566-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84566-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="84566-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84566-114">Not supported.</span></span>|
|<span data-ttu-id="84566-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="84566-115">Application</span></span>|<span data-ttu-id="84566-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84566-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="84566-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="84566-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="84566-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="84566-118">Global administrator</span></span>
* <span data-ttu-id="84566-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="84566-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="84566-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84566-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="84566-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84566-121">Request headers</span></span>

|<span data-ttu-id="84566-122">Имя</span><span class="sxs-lookup"><span data-stu-id="84566-122">Name</span></span>|<span data-ttu-id="84566-123">Описание</span><span class="sxs-lookup"><span data-stu-id="84566-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="84566-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84566-124">Authorization</span></span>|<span data-ttu-id="84566-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84566-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="84566-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84566-127">Content-Type</span></span>|<span data-ttu-id="84566-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84566-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84566-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84566-130">Request body</span></span>

<span data-ttu-id="84566-131">В теле запроса предостерегать представление [JSON b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="84566-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="84566-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="84566-132">Property</span></span>|<span data-ttu-id="84566-133">Тип</span><span class="sxs-lookup"><span data-stu-id="84566-133">Type</span></span>|<span data-ttu-id="84566-134">Описание</span><span class="sxs-lookup"><span data-stu-id="84566-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84566-135">id</span><span class="sxs-lookup"><span data-stu-id="84566-135">id</span></span>|<span data-ttu-id="84566-136">String</span><span class="sxs-lookup"><span data-stu-id="84566-136">String</span></span>|<span data-ttu-id="84566-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84566-137">Required.</span></span> <span data-ttu-id="84566-138">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="84566-138">The name of the user flow.</span></span> <span data-ttu-id="84566-139">После создания имя будет предварительно заранее. `B2C_1`</span><span class="sxs-lookup"><span data-stu-id="84566-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="84566-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="84566-140">userFlowType</span></span>|<span data-ttu-id="84566-141">String</span><span class="sxs-lookup"><span data-stu-id="84566-141">String</span></span>|<span data-ttu-id="84566-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84566-142">Required.</span></span> <span data-ttu-id="84566-143">Тип пользовательского потока, который вы создаете.</span><span class="sxs-lookup"><span data-stu-id="84566-143">The type of user flow you are creating.</span></span> <span data-ttu-id="84566-144">Поддерживаемые значения для **userFlowType**:</span><span class="sxs-lookup"><span data-stu-id="84566-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="84566-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="84566-145">userFlowTypeVersion</span></span>|<span data-ttu-id="84566-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="84566-146">Float</span></span>|<span data-ttu-id="84566-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="84566-147">Required.</span></span> <span data-ttu-id="84566-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="84566-148">The version of the user flow.</span></span>|
|<span data-ttu-id="84566-149">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="84566-149">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="84566-150">Логический</span><span class="sxs-lookup"><span data-stu-id="84566-150">Boolean</span></span>|<span data-ttu-id="84566-151">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="84566-151">Optional.</span></span> <span data-ttu-id="84566-152">Определяет, включена ли настройка языка в потоке пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="84566-152">Determines whether language customization is enabled within the Azure AD B2C user flow.</span></span> <span data-ttu-id="84566-153">Настройка языка не включена по умолчанию для потоков пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="84566-153">Language customization is not enabled by default for Azure AD B2C user flows.</span></span>|
|<span data-ttu-id="84566-154">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="84566-154">defaultLanguageTag</span></span>|<span data-ttu-id="84566-155">String</span><span class="sxs-lookup"><span data-stu-id="84566-155">String</span></span>|<span data-ttu-id="84566-156">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="84566-156">Optional.</span></span>  <span data-ttu-id="84566-157">Указывает язык по умолчанию b2cIdentityUserFlow, который используется, когда в запросе не указан `ui_locale` тег.</span><span class="sxs-lookup"><span data-stu-id="84566-157">Specifies the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="84566-158">Это поле соответствует спецификации [RFC 5646](https://tools.ietf.org/html/rfc5646).</span><span class="sxs-lookup"><span data-stu-id="84566-158">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|
|<span data-ttu-id="84566-159">identityProviders</span><span class="sxs-lookup"><span data-stu-id="84566-159">identityProviders</span></span>|<span data-ttu-id="84566-160">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="84566-160">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="84566-161">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="84566-161">Optional.</span></span> <span data-ttu-id="84566-162">Поставщики удостоверений, которые необходимо включить в поток пользователей.</span><span class="sxs-lookup"><span data-stu-id="84566-162">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="84566-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="84566-163">Response</span></span>

<span data-ttu-id="84566-164">В случае успешной работы этот метод возвращает код отклика и заголовку Location с URI на объект `201 Created` [b2cIdentityUserFlow,](../resources/b2cidentityuserflow.md) созданный для этого запроса, с префиксом, добавленным в `B2C_1` имя.</span><span class="sxs-lookup"><span data-stu-id="84566-164">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="84566-165">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="84566-165">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="84566-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="84566-166">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="84566-167">Пример 1. Создание пользовательского потока со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="84566-167">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="84566-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="84566-168">Request</span></span>

<span data-ttu-id="84566-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84566-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84566-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="84566-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3
}
```

# <a name="c"></a>[<span data-ttu-id="84566-171">C#</span><span class="sxs-lookup"><span data-stu-id="84566-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84566-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84566-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84566-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84566-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84566-174">Java</span><span class="sxs-lookup"><span data-stu-id="84566-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="84566-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="84566-175">Response</span></span>

<span data-ttu-id="84566-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84566-176">The following is an example of the response.</span></span>

<span data-ttu-id="84566-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="84566-177">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer
Content-type: application/json

{
    "id": "B2C_1_Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3,
    "isLanguageCustomizationEnabled": false,
    "defaultLanguageTag": "en"
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="84566-178">Пример 2. Создание пользовательского потока со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="84566-178">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="84566-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="84566-179">Request</span></span>

<span data-ttu-id="84566-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84566-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84566-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="84566-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows_identityProvider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3,
    "identityProviders": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "Name": "Facebook"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="84566-182">C#</span><span class="sxs-lookup"><span data-stu-id="84566-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84566-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84566-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84566-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84566-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84566-185">Java</span><span class="sxs-lookup"><span data-stu-id="84566-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84566-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="84566-186">Response</span></span>

<span data-ttu-id="84566-187">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84566-187">The following is an example of the response.</span></span>

<span data-ttu-id="84566-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="84566-188">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer
Content-type: application/json

{
    "id": "B2C_1_Customer",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 3,
    "isLanguageCustomizationEnabled": false,
    "defaultLanguageTag": "en"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2CUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2cUserFlow_from_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '3'",
    "Error: create_b2cUserFlow_from_b2cUserFlows_identityProvider/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '3'"
  ]
}-->

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="84566-189">Пример 3. Создание пользовательского потока с значениями по умолчанию и конфигурацией для соединителов API</span><span class="sxs-lookup"><span data-stu-id="84566-189">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="84566-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="84566-190">Request</span></span>

<span data-ttu-id="84566-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84566-191">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="84566-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="84566-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2cuserflow_from_b2cuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration":{
        "postFederationSignup":{
            "@odata.id": "{apiConnectorId}"
        },
        "postAttributeCollection":{
            "@odata.id": "{apiConnectorId}"
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="84566-193">C#</span><span class="sxs-lookup"><span data-stu-id="84566-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84566-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84566-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84566-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84566-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84566-196">Java</span><span class="sxs-lookup"><span data-stu-id="84566-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84566-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="84566-197">Response</span></span>

<span data-ttu-id="84566-198">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84566-198">The following is an example of the response.</span></span>

<span data-ttu-id="84566-199">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="84566-199">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="84566-200">**Примечание:** Свойство `apiConnectorConfiguration` всегда возвращает значение {} '.</span><span class="sxs-lookup"><span data-stu-id="84566-200">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="84566-201">Чтобы увидеть полное значение свойств навигации, используйте [этот](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span><span class="sxs-lookup"><span data-stu-id="84566-201">To see full value with the navigation properties, use [this](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows/$entity",
    "id": "B2C_1_UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration": {}
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2cUserFlow_from_b2cuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
