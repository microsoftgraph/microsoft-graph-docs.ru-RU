---
title: Создание объекта b2cIdentityUserFlow
description: Создание объекта b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0537eaf5baea543ee4cf9dbbd24b8cb80fc4d48d
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844236"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="95a02-103">Создание объекта b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="95a02-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="95a02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95a02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95a02-105">Создание объекта [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="95a02-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95a02-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95a02-106">Permissions</span></span>

<span data-ttu-id="95a02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95a02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95a02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95a02-109">Permission type</span></span>      | <span data-ttu-id="95a02-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95a02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95a02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95a02-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95a02-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95a02-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="95a02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95a02-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="95a02-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95a02-114">Not supported.</span></span>|
|<span data-ttu-id="95a02-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="95a02-115">Application</span></span>|<span data-ttu-id="95a02-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95a02-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="95a02-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="95a02-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="95a02-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="95a02-118">Global administrator</span></span>
* <span data-ttu-id="95a02-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="95a02-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="95a02-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95a02-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="95a02-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95a02-121">Request headers</span></span>

|<span data-ttu-id="95a02-122">Имя</span><span class="sxs-lookup"><span data-stu-id="95a02-122">Name</span></span>|<span data-ttu-id="95a02-123">Описание</span><span class="sxs-lookup"><span data-stu-id="95a02-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="95a02-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95a02-124">Authorization</span></span>|<span data-ttu-id="95a02-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95a02-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="95a02-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95a02-127">Content-Type</span></span>|<span data-ttu-id="95a02-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95a02-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95a02-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95a02-130">Request body</span></span>

<span data-ttu-id="95a02-131">В теле запроса предостерегать представление [объекта b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)в JSON.</span><span class="sxs-lookup"><span data-stu-id="95a02-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="95a02-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="95a02-132">Property</span></span>|<span data-ttu-id="95a02-133">Тип</span><span class="sxs-lookup"><span data-stu-id="95a02-133">Type</span></span>|<span data-ttu-id="95a02-134">Описание</span><span class="sxs-lookup"><span data-stu-id="95a02-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95a02-135">id</span><span class="sxs-lookup"><span data-stu-id="95a02-135">id</span></span>|<span data-ttu-id="95a02-136">String</span><span class="sxs-lookup"><span data-stu-id="95a02-136">String</span></span>|<span data-ttu-id="95a02-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95a02-137">Required.</span></span> <span data-ttu-id="95a02-138">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="95a02-138">The name of the user flow.</span></span> <span data-ttu-id="95a02-139">Имя будет предварительно замещено после `B2C_1` создания.</span><span class="sxs-lookup"><span data-stu-id="95a02-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="95a02-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="95a02-140">userFlowType</span></span>|<span data-ttu-id="95a02-141">String</span><span class="sxs-lookup"><span data-stu-id="95a02-141">String</span></span>|<span data-ttu-id="95a02-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95a02-142">Required.</span></span> <span data-ttu-id="95a02-143">Тип создаемого пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="95a02-143">The type of user flow you are creating.</span></span> <span data-ttu-id="95a02-144">Поддерживаемые значения для **userFlowType**:</span><span class="sxs-lookup"><span data-stu-id="95a02-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="95a02-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="95a02-145">userFlowTypeVersion</span></span>|<span data-ttu-id="95a02-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="95a02-146">Float</span></span>|<span data-ttu-id="95a02-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95a02-147">Required.</span></span> <span data-ttu-id="95a02-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="95a02-148">The version of the user flow.</span></span>|
|<span data-ttu-id="95a02-149">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="95a02-149">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="95a02-150">Логический</span><span class="sxs-lookup"><span data-stu-id="95a02-150">Boolean</span></span>|<span data-ttu-id="95a02-151">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="95a02-151">Optional.</span></span> <span data-ttu-id="95a02-152">Определяет, включена ли настройка языка в пользовательском потоке B2C Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95a02-152">Determines whether language customization is enabled within the Azure AD B2C user flow.</span></span> <span data-ttu-id="95a02-153">Настройка языка не включена по умолчанию для потоков пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="95a02-153">Language customization is not enabled by default for Azure AD B2C user flows.</span></span>|
|<span data-ttu-id="95a02-154">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="95a02-154">defaultLanguageTag</span></span>|<span data-ttu-id="95a02-155">String</span><span class="sxs-lookup"><span data-stu-id="95a02-155">String</span></span>|<span data-ttu-id="95a02-156">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="95a02-156">Optional.</span></span>  <span data-ttu-id="95a02-157">Указывает язык по умолчанию для b2cIdentityUserFlow, который используется, когда в запросе не указан `ui_locale` тег.</span><span class="sxs-lookup"><span data-stu-id="95a02-157">Specifies the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="95a02-158">Это поле соответствует спецификации [RFC 5646](https://tools.ietf.org/html/rfc5646).</span><span class="sxs-lookup"><span data-stu-id="95a02-158">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|
|<span data-ttu-id="95a02-159">identityProviders</span><span class="sxs-lookup"><span data-stu-id="95a02-159">identityProviders</span></span>|<span data-ttu-id="95a02-160">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="95a02-160">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="95a02-161">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="95a02-161">Optional.</span></span> <span data-ttu-id="95a02-162">Поставщики удостоверений, которые необходимо включить в поток пользователей.</span><span class="sxs-lookup"><span data-stu-id="95a02-162">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="95a02-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="95a02-163">Response</span></span>

<span data-ttu-id="95a02-164">В случае успеха этот метод возвращает код ответа и заголовщик Location с `201 Created` URI [объекту b2cIdentityUserFlow,](../resources/b2cidentityuserflow.md) созданному для этого запроса, с префиксом, добавленным к `B2C_1` имени.</span><span class="sxs-lookup"><span data-stu-id="95a02-164">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="95a02-165">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="95a02-165">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="95a02-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="95a02-166">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="95a02-167">Пример 1. Создание пользовательского потока со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="95a02-167">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="95a02-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="95a02-168">Request</span></span>

<span data-ttu-id="95a02-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95a02-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95a02-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="95a02-170">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="95a02-171">C#</span><span class="sxs-lookup"><span data-stu-id="95a02-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95a02-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95a02-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95a02-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95a02-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95a02-174">Java</span><span class="sxs-lookup"><span data-stu-id="95a02-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="95a02-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="95a02-175">Response</span></span>

<span data-ttu-id="95a02-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="95a02-176">The following is an example of the response.</span></span>

<span data-ttu-id="95a02-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95a02-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="95a02-178">Пример 2. Создание пользовательского потока со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="95a02-178">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="95a02-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="95a02-179">Request</span></span>

<span data-ttu-id="95a02-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95a02-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95a02-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="95a02-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="95a02-182">C#</span><span class="sxs-lookup"><span data-stu-id="95a02-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95a02-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95a02-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95a02-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95a02-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95a02-185">Java</span><span class="sxs-lookup"><span data-stu-id="95a02-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95a02-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="95a02-186">Response</span></span>

<span data-ttu-id="95a02-187">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="95a02-187">The following is an example of the response.</span></span>

<span data-ttu-id="95a02-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95a02-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="95a02-189">Пример 3. Создание пользовательского потока со значениями по умолчанию и конфигурацией для соединителов API</span><span class="sxs-lookup"><span data-stu-id="95a02-189">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="95a02-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="95a02-190">Request</span></span>

<span data-ttu-id="95a02-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95a02-191">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="95a02-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="95a02-192">HTTP</span></span>](#tab/http)
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
            "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"
        },
        "postAttributeCollection":{
            "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"
        }
    }
}
```
# <a name="c"></a>[<span data-ttu-id="95a02-193">C#</span><span class="sxs-lookup"><span data-stu-id="95a02-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95a02-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95a02-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95a02-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95a02-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95a02-196">Java</span><span class="sxs-lookup"><span data-stu-id="95a02-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="95a02-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="95a02-197">Response</span></span>

<span data-ttu-id="95a02-198">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="95a02-198">The following is an example of the response.</span></span>

<span data-ttu-id="95a02-199">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95a02-199">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="95a02-200">**Примечание.** Свойство всегда возвращает значение `apiConnectorConfiguration` {} '.</span><span class="sxs-lookup"><span data-stu-id="95a02-200">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="95a02-201">Чтобы увидеть полное значение свойств навигации, [используйте](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) этот API.</span><span class="sxs-lookup"><span data-stu-id="95a02-201">To see full value with the navigation properties, use [this](../api/b2cidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

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
    "Error: create_b2cUserFlow_from_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2cUserFlow_from_b2cUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2cUserFlow_from_b2cuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
