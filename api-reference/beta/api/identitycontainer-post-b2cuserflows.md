---
title: Создание b2cIdentityUserFlow
description: Создание нового объекта b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c110d8bc1db9ace9375a0bae77937ab79ef1eb3a
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406477"
---
# <a name="create-b2cidentityuserflow"></a><span data-ttu-id="ee363-103">Создание b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="ee363-103">Create b2cIdentityUserFlow</span></span>

<span data-ttu-id="ee363-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee363-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee363-105">Создание нового объекта [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="ee363-105">Create a new [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee363-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee363-106">Permissions</span></span>

<span data-ttu-id="ee363-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee363-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee363-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee363-109">Permission type</span></span>      | <span data-ttu-id="ee363-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee363-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee363-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee363-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee363-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ee363-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ee363-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee363-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ee363-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee363-114">Not supported.</span></span>|
|<span data-ttu-id="ee363-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee363-115">Application</span></span>|<span data-ttu-id="ee363-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ee363-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ee363-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ee363-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ee363-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ee363-118">Global administrator</span></span>
* <span data-ttu-id="ee363-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="ee363-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ee363-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee363-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="ee363-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee363-121">Request headers</span></span>

|<span data-ttu-id="ee363-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ee363-122">Name</span></span>|<span data-ttu-id="ee363-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ee363-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ee363-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee363-124">Authorization</span></span>|<span data-ttu-id="ee363-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee363-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ee363-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee363-127">Content-Type</span></span>|<span data-ttu-id="ee363-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee363-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee363-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee363-130">Request body</span></span>

<span data-ttu-id="ee363-131">В тексте запроса предоставьте представление объекта [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee363-131">In the request body, provide a JSON representation of a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

|<span data-ttu-id="ee363-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee363-132">Property</span></span>|<span data-ttu-id="ee363-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ee363-133">Type</span></span>|<span data-ttu-id="ee363-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ee363-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee363-135">id</span><span class="sxs-lookup"><span data-stu-id="ee363-135">id</span></span>|<span data-ttu-id="ee363-136">String</span><span class="sxs-lookup"><span data-stu-id="ee363-136">String</span></span>|<span data-ttu-id="ee363-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee363-137">Required.</span></span> <span data-ttu-id="ee363-138">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="ee363-138">The name of the user flow.</span></span> <span data-ttu-id="ee363-139">Имя будет предваряться `B2C_1` после создания.</span><span class="sxs-lookup"><span data-stu-id="ee363-139">The name will be pre-pended with `B2C_1` after creation.</span></span>|
|<span data-ttu-id="ee363-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="ee363-140">userFlowType</span></span>|<span data-ttu-id="ee363-141">String</span><span class="sxs-lookup"><span data-stu-id="ee363-141">String</span></span>|<span data-ttu-id="ee363-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee363-142">Required.</span></span> <span data-ttu-id="ee363-143">Тип создаваемого пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="ee363-143">The type of user flow you are creating.</span></span> <span data-ttu-id="ee363-144">Поддерживаемые значения для **userFlowType**:</span><span class="sxs-lookup"><span data-stu-id="ee363-144">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="ee363-145">усерфловтипеверсион</span><span class="sxs-lookup"><span data-stu-id="ee363-145">userFlowTypeVersion</span></span>|<span data-ttu-id="ee363-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="ee363-146">Float</span></span>|<span data-ttu-id="ee363-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="ee363-147">Required.</span></span> <span data-ttu-id="ee363-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="ee363-148">The version of the user flow.</span></span>|
|<span data-ttu-id="ee363-149">identityProviders</span><span class="sxs-lookup"><span data-stu-id="ee363-149">identityProviders</span></span>|<span data-ttu-id="ee363-150">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="ee363-150">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="ee363-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ee363-151">Optional.</span></span> <span data-ttu-id="ee363-152">Поставщики удостоверений, которые необходимо включить в пользовательский блок.</span><span class="sxs-lookup"><span data-stu-id="ee363-152">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="ee363-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee363-153">Response</span></span>

<span data-ttu-id="ee363-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и заголовок Location с URI для объекта [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) , созданного для этого запроса, с `B2C_1` префиксом, добавленным к имени.</span><span class="sxs-lookup"><span data-stu-id="ee363-154">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object created for this request, with the `B2C_1` prefix added to the name.</span></span> <span data-ttu-id="ee363-155">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="ee363-155">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="ee363-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="ee363-156">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="ee363-157">Пример 1: создание пользовательского процесса со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="ee363-157">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="ee363-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee363-158">Request</span></span>

<span data-ttu-id="ee363-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee363-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee363-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee363-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ee363-161">C#</span><span class="sxs-lookup"><span data-stu-id="ee363-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee363-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee363-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee363-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee363-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ee363-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee363-164">Response</span></span>

<span data-ttu-id="ee363-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ee363-165">The following is an example of the response.</span></span>

<span data-ttu-id="ee363-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ee363-166">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "userFlowTypeVersion": 3
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="ee363-167">Пример 2: создание пользовательского процесса со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="ee363-167">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="ee363-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee363-168">Request</span></span>

<span data-ttu-id="ee363-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee363-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee363-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee363-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ee363-171">C#</span><span class="sxs-lookup"><span data-stu-id="ee363-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2cuserflow-from-b2cuserflows-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee363-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee363-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2cuserflow-from-b2cuserflows-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee363-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee363-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2cuserflow-from-b2cuserflows-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ee363-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee363-174">Response</span></span>

<span data-ttu-id="ee363-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ee363-175">The following is an example of the response.</span></span>

<span data-ttu-id="ee363-176">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ee363-176">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "userFlowTypeVersion": 3
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


