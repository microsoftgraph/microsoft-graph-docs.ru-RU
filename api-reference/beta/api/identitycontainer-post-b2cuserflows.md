---
title: Создание объекта b2cIdentityUserFlow
description: Создание объекта b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 98d603632e724817cec2d4c97e06389608cc3f10
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705872"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="ce6a3-103">Создание объекта b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="ce6a3-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="ce6a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce6a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce6a3-105">Создание объекта [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="ce6a3-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce6a3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce6a3-106">Permissions</span></span>

<span data-ttu-id="ce6a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce6a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce6a3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce6a3-109">Permission type</span></span>      | <span data-ttu-id="ce6a3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce6a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce6a3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce6a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce6a3-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6a3-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ce6a3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce6a3-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ce6a3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-114">Not supported.</span></span>|
|<span data-ttu-id="ce6a3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce6a3-115">Application</span></span>|<span data-ttu-id="ce6a3-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce6a3-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ce6a3-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ce6a3-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ce6a3-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ce6a3-118">Global administrator</span></span>
* <span data-ttu-id="ce6a3-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="ce6a3-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ce6a3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce6a3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="ce6a3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce6a3-121">Request headers</span></span>

|<span data-ttu-id="ce6a3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ce6a3-122">Name</span></span>|<span data-ttu-id="ce6a3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ce6a3-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ce6a3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce6a3-124">Authorization</span></span>|<span data-ttu-id="ce6a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce6a3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce6a3-127">Content-Type</span></span>|<span data-ttu-id="ce6a3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce6a3-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce6a3-130">Request body</span></span>

<span data-ttu-id="ce6a3-131">В теле запроса предостерегать представление [объекта b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)в JSON.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="ce6a3-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce6a3-132">Property</span></span>|<span data-ttu-id="ce6a3-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ce6a3-133">Type</span></span>|<span data-ttu-id="ce6a3-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ce6a3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce6a3-135">id</span><span class="sxs-lookup"><span data-stu-id="ce6a3-135">id</span></span>|<span data-ttu-id="ce6a3-136">String</span><span class="sxs-lookup"><span data-stu-id="ce6a3-136">String</span></span>|<span data-ttu-id="ce6a3-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-137">Required.</span></span> <span data-ttu-id="ce6a3-138">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-138">The name of the user flow.</span></span> <span data-ttu-id="ce6a3-139">Имя будет предварительно замещено после `B2C_1` создания.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="ce6a3-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="ce6a3-140">userFlowType</span></span>|<span data-ttu-id="ce6a3-141">String</span><span class="sxs-lookup"><span data-stu-id="ce6a3-141">String</span></span>|<span data-ttu-id="ce6a3-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-142">Required.</span></span> <span data-ttu-id="ce6a3-143">Тип создаемого пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-143">The type of user flow you are creating.</span></span> <span data-ttu-id="ce6a3-144">Поддерживаемые значения для **userFlowType**:</span><span class="sxs-lookup"><span data-stu-id="ce6a3-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="ce6a3-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ce6a3-145">userFlowTypeVersion</span></span>|<span data-ttu-id="ce6a3-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="ce6a3-146">Float</span></span>|<span data-ttu-id="ce6a3-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-147">Required.</span></span> <span data-ttu-id="ce6a3-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-148">The version of the user flow.</span></span>|
|<span data-ttu-id="ce6a3-149">isLanguageCustomizationEnabled</span><span class="sxs-lookup"><span data-stu-id="ce6a3-149">isLanguageCustomizationEnabled</span></span>|<span data-ttu-id="ce6a3-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6a3-150">Boolean</span></span>|<span data-ttu-id="ce6a3-151">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-151">Optional.</span></span> <span data-ttu-id="ce6a3-152">Определяет, включена ли настройка языка в пользовательском потоке B2C Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-152">Determines whether language customization is enabled within the Azure AD B2C user flow.</span></span> <span data-ttu-id="ce6a3-153">Настройка языка не включена по умолчанию для потоков пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-153">Language customization is not enabled by default for Azure AD B2C user flows.</span></span>|
|<span data-ttu-id="ce6a3-154">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="ce6a3-154">defaultLanguageTag</span></span>|<span data-ttu-id="ce6a3-155">String</span><span class="sxs-lookup"><span data-stu-id="ce6a3-155">String</span></span>|<span data-ttu-id="ce6a3-156">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-156">Optional.</span></span>  <span data-ttu-id="ce6a3-157">Указывает язык по умолчанию для b2cIdentityUserFlow, который используется, когда в запросе не указан `ui_locale` тег.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-157">Specifies the default language of the b2cIdentityUserFlow that is used when no `ui_locale` tag is specified in the request.</span></span> <span data-ttu-id="ce6a3-158">Это поле соответствует [стандарту RFC 5646.](https://tools.ietf.org/html/rfc5646)</span><span class="sxs-lookup"><span data-stu-id="ce6a3-158">This field is [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant.</span></span>|
|<span data-ttu-id="ce6a3-159">identityProviders</span><span class="sxs-lookup"><span data-stu-id="ce6a3-159">identityProviders</span></span>|<span data-ttu-id="ce6a3-160">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="ce6a3-160">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="ce6a3-161">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-161">Optional.</span></span> <span data-ttu-id="ce6a3-162">Поставщики удостоверений, которые необходимо включить в поток пользователей.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-162">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="ce6a3-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce6a3-163">Response</span></span>

<span data-ttu-id="ce6a3-164">В случае успеха этот метод возвращает код отклика и заголовщик Location с `201 Created` URI [объекту b2cIdentityUserFlow,](../resources/b2cidentityuserflow.md) созданному для этого запроса, с префиксом, добавленным к `B2C_1` имени.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-164">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="ce6a3-165">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-165">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="ce6a3-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="ce6a3-166">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="ce6a3-167">Пример 1. Создание пользовательского потока со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="ce6a3-167">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="ce6a3-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce6a3-168">Request</span></span>

<span data-ttu-id="ce6a3-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce6a3-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce6a3-170">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="ce6a3-171">C#</span><span class="sxs-lookup"><span data-stu-id="ce6a3-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce6a3-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce6a3-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce6a3-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6a3-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce6a3-174">Java</span><span class="sxs-lookup"><span data-stu-id="ce6a3-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ce6a3-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce6a3-175">Response</span></span>

<span data-ttu-id="ce6a3-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-176">The following is an example of the response.</span></span>

<span data-ttu-id="ce6a3-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="ce6a3-178">Пример 2. Создание пользовательского потока со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="ce6a3-178">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="ce6a3-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce6a3-179">Request</span></span>

<span data-ttu-id="ce6a3-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce6a3-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce6a3-181">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ce6a3-182">C#</span><span class="sxs-lookup"><span data-stu-id="ce6a3-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce6a3-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce6a3-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce6a3-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce6a3-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce6a3-185">Java</span><span class="sxs-lookup"><span data-stu-id="ce6a3-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-b2cuserflow-from-b2cuserflows-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ce6a3-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce6a3-186">Response</span></span>

<span data-ttu-id="ce6a3-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-187">The following is an example of the response.</span></span>

<span data-ttu-id="ce6a3-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ce6a3-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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
