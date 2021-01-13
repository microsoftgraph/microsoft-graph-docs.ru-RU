---
title: Создание объекта b2xIdentityUserFlow
description: Создание объекта b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f64b29b242f92caf59a9318caff89f9b401a120e
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844400"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="9edc6-103">Создание объекта b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="9edc6-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="9edc6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9edc6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9edc6-105">Создание объекта [b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="9edc6-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9edc6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9edc6-106">Permissions</span></span>

<span data-ttu-id="9edc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9edc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9edc6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9edc6-109">Permission type</span></span>      | <span data-ttu-id="9edc6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9edc6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9edc6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9edc6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9edc6-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9edc6-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9edc6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9edc6-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9edc6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9edc6-114">Not supported.</span></span>|
|<span data-ttu-id="9edc6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9edc6-115">Application</span></span>|<span data-ttu-id="9edc6-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9edc6-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9edc6-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="9edc6-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9edc6-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9edc6-118">Global administrator</span></span>
* <span data-ttu-id="9edc6-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="9edc6-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9edc6-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9edc6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="9edc6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9edc6-121">Request headers</span></span>

|<span data-ttu-id="9edc6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9edc6-122">Name</span></span>|<span data-ttu-id="9edc6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9edc6-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9edc6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9edc6-124">Authorization</span></span>|<span data-ttu-id="9edc6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9edc6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9edc6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9edc6-127">Content-Type</span></span>|<span data-ttu-id="9edc6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9edc6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9edc6-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9edc6-130">Request body</span></span>

<span data-ttu-id="9edc6-131">В теле запроса предостерегать представление [объекта b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)в JSON.</span><span class="sxs-lookup"><span data-stu-id="9edc6-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="9edc6-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="9edc6-132">Property</span></span>|<span data-ttu-id="9edc6-133">Тип</span><span class="sxs-lookup"><span data-stu-id="9edc6-133">Type</span></span>|<span data-ttu-id="9edc6-134">Описание</span><span class="sxs-lookup"><span data-stu-id="9edc6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9edc6-135">id</span><span class="sxs-lookup"><span data-stu-id="9edc6-135">id</span></span>|<span data-ttu-id="9edc6-136">String</span><span class="sxs-lookup"><span data-stu-id="9edc6-136">String</span></span>|<span data-ttu-id="9edc6-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9edc6-137">Required.</span></span> <span data-ttu-id="9edc6-138">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="9edc6-138">The name of the user flow.</span></span> <span data-ttu-id="9edc6-139">Имя будет предварительно замещено после `B2X_1` создания.</span><span class="sxs-lookup"><span data-stu-id="9edc6-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="9edc6-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="9edc6-140">userFlowType</span></span>|<span data-ttu-id="9edc6-141">String</span><span class="sxs-lookup"><span data-stu-id="9edc6-141">String</span></span>|<span data-ttu-id="9edc6-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9edc6-142">Required.</span></span> <span data-ttu-id="9edc6-143">Тип создаемого пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="9edc6-143">The type of user flow you are creating.</span></span> <span data-ttu-id="9edc6-144">Это значение всегда будет `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="9edc6-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="9edc6-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="9edc6-145">userFlowTypeVersion</span></span>|<span data-ttu-id="9edc6-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="9edc6-146">Float</span></span>|<span data-ttu-id="9edc6-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9edc6-147">Required.</span></span> <span data-ttu-id="9edc6-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="9edc6-148">The version of the user flow.</span></span> <span data-ttu-id="9edc6-149">Это значение всегда будет 1.</span><span class="sxs-lookup"><span data-stu-id="9edc6-149">This value will always be 1.</span></span>|
|<span data-ttu-id="9edc6-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="9edc6-150">identityProviders</span></span>|<span data-ttu-id="9edc6-151">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="9edc6-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="9edc6-152">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="9edc6-152">Optional.</span></span> <span data-ttu-id="9edc6-153">Поставщики удостоверений, которые необходимо включить в поток пользователей.</span><span class="sxs-lookup"><span data-stu-id="9edc6-153">The identity providers you want to include in the user flow.</span></span>|
|<span data-ttu-id="9edc6-154">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="9edc6-154">apiConnectorConfiguration</span></span>|[<span data-ttu-id="9edc6-155">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="9edc6-155">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="9edc6-156">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="9edc6-156">Optional.</span></span> <span data-ttu-id="9edc6-157">Настройка для включения соединителя API с целью использования в составе пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="9edc6-157">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="9edc6-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="9edc6-158">Response</span></span>

<span data-ttu-id="9edc6-159">В случае успеха этот метод возвращает код отклика и заголовщик Location с `201 Created` URI [объекту b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) созданному для этого запроса, с префиксом, добавленным к `B2X_1` имени.</span><span class="sxs-lookup"><span data-stu-id="9edc6-159">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="9edc6-160">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="9edc6-160">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="9edc6-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="9edc6-161">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="9edc6-162">Пример 1. Создание пользовательского потока со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="9edc6-162">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="9edc6-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="9edc6-163">Request</span></span>

<span data-ttu-id="9edc6-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9edc6-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9edc6-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="9edc6-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```
# <a name="c"></a>[<span data-ttu-id="9edc6-166">C#</span><span class="sxs-lookup"><span data-stu-id="9edc6-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9edc6-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9edc6-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9edc6-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9edc6-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9edc6-169">Java</span><span class="sxs-lookup"><span data-stu-id="9edc6-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9edc6-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="9edc6-170">Response</span></span>

<span data-ttu-id="9edc6-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9edc6-171">The following is an example of the response.</span></span>

<span data-ttu-id="9edc6-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9edc6-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="9edc6-173">Пример 2. Создание пользовательского потока со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="9edc6-173">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="9edc6-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="9edc6-174">Request</span></span>

<span data-ttu-id="9edc6-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9edc6-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9edc6-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="9edc6-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_identityProviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "identityProviders": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="9edc6-177">C#</span><span class="sxs-lookup"><span data-stu-id="9edc6-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9edc6-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9edc6-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9edc6-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9edc6-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9edc6-180">Java</span><span class="sxs-lookup"><span data-stu-id="9edc6-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9edc6-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="9edc6-181">Response</span></span>

<span data-ttu-id="9edc6-182">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9edc6-182">The following is an example of the response.</span></span>

<span data-ttu-id="9edc6-183">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9edc6-183">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="9edc6-184">Пример 3. Создание пользовательского потока со значениями по умолчанию и конфигурацией для соединителов API</span><span class="sxs-lookup"><span data-stu-id="9edc6-184">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="9edc6-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="9edc6-185">Request</span></span>

<span data-ttu-id="9edc6-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9edc6-186">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9edc6-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="9edc6-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
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
# <a name="c"></a>[<span data-ttu-id="9edc6-188">C#</span><span class="sxs-lookup"><span data-stu-id="9edc6-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-apiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9edc6-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9edc6-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-apiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9edc6-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9edc6-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-apiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9edc6-191">Java</span><span class="sxs-lookup"><span data-stu-id="9edc6-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-apiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9edc6-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="9edc6-192">Response</span></span>

<span data-ttu-id="9edc6-193">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9edc6-193">The following is an example of the response.</span></span>

<span data-ttu-id="9edc6-194">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9edc6-194">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="9edc6-195">**Примечание.** Свойство всегда возвращает значение `apiConnectorConfiguration` {} '.</span><span class="sxs-lookup"><span data-stu-id="9edc6-195">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="9edc6-196">Чтобы увидеть полное значение свойств навигации, [используйте](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) этот API.</span><span class="sxs-lookup"><span data-stu-id="9edc6-196">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows/$entity",
    "id": "B2X_1_UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration": {}
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2xUserFlow_from_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
