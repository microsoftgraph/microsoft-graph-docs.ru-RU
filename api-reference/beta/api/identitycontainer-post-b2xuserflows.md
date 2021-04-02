---
title: Создание b2xIdentityUserFlow
description: Создайте новый объект b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 0eaabe737d6bc656c5f644dac3ca2903fc39bfd6
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508592"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="8d869-103">Создание b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="8d869-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="8d869-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d869-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d869-105">Создайте [новый объект b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="8d869-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d869-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d869-106">Permissions</span></span>

<span data-ttu-id="8d869-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d869-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d869-109">Permission type</span></span>      | <span data-ttu-id="8d869-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d869-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d869-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d869-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d869-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d869-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="8d869-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d869-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8d869-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d869-114">Not supported.</span></span>|
|<span data-ttu-id="8d869-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d869-115">Application</span></span>|<span data-ttu-id="8d869-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d869-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8d869-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="8d869-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8d869-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8d869-118">Global administrator</span></span>
* <span data-ttu-id="8d869-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="8d869-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8d869-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d869-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="8d869-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d869-121">Request headers</span></span>

|<span data-ttu-id="8d869-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8d869-122">Name</span></span>|<span data-ttu-id="8d869-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8d869-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8d869-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d869-124">Authorization</span></span>|<span data-ttu-id="8d869-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d869-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8d869-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d869-127">Content-Type</span></span>|<span data-ttu-id="8d869-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d869-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d869-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d869-130">Request body</span></span>

<span data-ttu-id="8d869-131">В теле запроса предостерегать представление [JSON b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="8d869-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="8d869-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d869-132">Property</span></span>|<span data-ttu-id="8d869-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8d869-133">Type</span></span>|<span data-ttu-id="8d869-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8d869-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d869-135">id</span><span class="sxs-lookup"><span data-stu-id="8d869-135">id</span></span>|<span data-ttu-id="8d869-136">String</span><span class="sxs-lookup"><span data-stu-id="8d869-136">String</span></span>|<span data-ttu-id="8d869-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d869-137">Required.</span></span> <span data-ttu-id="8d869-138">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="8d869-138">The name of the user flow.</span></span> <span data-ttu-id="8d869-139">После создания имя будет предварительно заранее. `B2X_1`</span><span class="sxs-lookup"><span data-stu-id="8d869-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="8d869-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="8d869-140">userFlowType</span></span>|<span data-ttu-id="8d869-141">String</span><span class="sxs-lookup"><span data-stu-id="8d869-141">String</span></span>|<span data-ttu-id="8d869-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d869-142">Required.</span></span> <span data-ttu-id="8d869-143">Тип пользовательского потока, который вы создаете.</span><span class="sxs-lookup"><span data-stu-id="8d869-143">The type of user flow you are creating.</span></span> <span data-ttu-id="8d869-144">Это значение всегда будет `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="8d869-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="8d869-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8d869-145">userFlowTypeVersion</span></span>|<span data-ttu-id="8d869-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="8d869-146">Float</span></span>|<span data-ttu-id="8d869-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8d869-147">Required.</span></span> <span data-ttu-id="8d869-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="8d869-148">The version of the user flow.</span></span> <span data-ttu-id="8d869-149">Это значение всегда будет 1.</span><span class="sxs-lookup"><span data-stu-id="8d869-149">This value will always be 1.</span></span>|
|<span data-ttu-id="8d869-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="8d869-150">identityProviders</span></span>|<span data-ttu-id="8d869-151">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="8d869-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="8d869-152">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8d869-152">Optional.</span></span> <span data-ttu-id="8d869-153">Поставщики удостоверений, которые необходимо включить в поток пользователей.</span><span class="sxs-lookup"><span data-stu-id="8d869-153">The identity providers you want to include in the user flow.</span></span>|
|<span data-ttu-id="8d869-154">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d869-154">apiConnectorConfiguration</span></span>|[<span data-ttu-id="8d869-155">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d869-155">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="8d869-156">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8d869-156">Optional.</span></span> <span data-ttu-id="8d869-157">Настройка для включения соединителя API с целью использования в составе пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="8d869-157">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="8d869-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d869-158">Response</span></span>

<span data-ttu-id="8d869-159">В случае успеха этот метод возвращает код отклика и заголовку Location с URI на объект `201 Created` [b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) созданный для этого запроса, с префиксом, добавленным в `B2X_1` имя.</span><span class="sxs-lookup"><span data-stu-id="8d869-159">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="8d869-160">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="8d869-160">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="8d869-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d869-161">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="8d869-162">Пример 1. Создание пользовательского потока со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="8d869-162">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="8d869-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d869-163">Request</span></span>

<span data-ttu-id="8d869-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d869-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d869-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d869-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d869-166">C#</span><span class="sxs-lookup"><span data-stu-id="8d869-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d869-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d869-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d869-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d869-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d869-169">Java</span><span class="sxs-lookup"><span data-stu-id="8d869-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d869-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d869-170">Response</span></span>

<span data-ttu-id="8d869-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d869-171">The following is an example of the response.</span></span>

<span data-ttu-id="8d869-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d869-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="8d869-173">Пример 2. Создание пользовательского потока со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="8d869-173">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="8d869-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d869-174">Request</span></span>

<span data-ttu-id="8d869-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d869-175">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d869-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d869-176">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d869-177">C#</span><span class="sxs-lookup"><span data-stu-id="8d869-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d869-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d869-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d869-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d869-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d869-180">Java</span><span class="sxs-lookup"><span data-stu-id="8d869-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2xuserflow-from-b2xuserflows-identityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8d869-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d869-181">Response</span></span>

<span data-ttu-id="8d869-182">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d869-182">The following is an example of the response.</span></span>

<span data-ttu-id="8d869-183">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d869-183">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="8d869-184">Пример 3. Создание пользовательского потока с значениями по умолчанию и конфигурацией для соединителов API</span><span class="sxs-lookup"><span data-stu-id="8d869-184">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="8d869-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d869-185">Request</span></span>

<span data-ttu-id="8d869-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d869-186">The following is an example of the request.</span></span>

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
            "@odata.id": "{apiConnectorId}"
        },
        "postAttributeCollection":{
            "@odata.id": "{apiConnectorId}"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="8d869-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d869-187">Response</span></span>

<span data-ttu-id="8d869-188">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d869-188">The following is an example of the response.</span></span>

<span data-ttu-id="8d869-189">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d869-189">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="8d869-190">**Примечание:** Свойство `apiConnectorConfiguration` всегда возвращает значение {} '.</span><span class="sxs-lookup"><span data-stu-id="8d869-190">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="8d869-191">Чтобы увидеть полное значение свойств навигации, используйте [этот](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span><span class="sxs-lookup"><span data-stu-id="8d869-191">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

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
