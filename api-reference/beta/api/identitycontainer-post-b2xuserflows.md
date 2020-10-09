---
title: Создание b2xIdentityUserFlow
description: Создание нового объекта b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82fe1f9a825262deff595d636c5fbd899cc970b3
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406465"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="5653c-103">Создание b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="5653c-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="5653c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5653c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5653c-105">Создание нового объекта [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="5653c-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5653c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5653c-106">Permissions</span></span>

<span data-ttu-id="5653c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5653c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5653c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5653c-109">Permission type</span></span>      | <span data-ttu-id="5653c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5653c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5653c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5653c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5653c-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5653c-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5653c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5653c-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5653c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5653c-114">Not supported.</span></span>|
|<span data-ttu-id="5653c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5653c-115">Application</span></span>|<span data-ttu-id="5653c-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5653c-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5653c-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="5653c-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5653c-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5653c-118">Global administrator</span></span>
* <span data-ttu-id="5653c-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="5653c-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5653c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5653c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="5653c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5653c-121">Request headers</span></span>

|<span data-ttu-id="5653c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5653c-122">Name</span></span>|<span data-ttu-id="5653c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5653c-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="5653c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5653c-124">Authorization</span></span>|<span data-ttu-id="5653c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5653c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5653c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5653c-127">Content-Type</span></span>|<span data-ttu-id="5653c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5653c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5653c-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="5653c-130">Request body</span></span>

<span data-ttu-id="5653c-131">В тексте запроса предоставьте представление объекта [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5653c-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="5653c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="5653c-132">Property</span></span>|<span data-ttu-id="5653c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5653c-133">Type</span></span>|<span data-ttu-id="5653c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5653c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5653c-135">id</span><span class="sxs-lookup"><span data-stu-id="5653c-135">id</span></span>|<span data-ttu-id="5653c-136">String</span><span class="sxs-lookup"><span data-stu-id="5653c-136">String</span></span>|<span data-ttu-id="5653c-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5653c-137">Required.</span></span> <span data-ttu-id="5653c-138">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="5653c-138">The name of the user flow.</span></span> <span data-ttu-id="5653c-139">Имя будет предваряться `B2X_1` после создания.</span><span class="sxs-lookup"><span data-stu-id="5653c-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="5653c-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="5653c-140">userFlowType</span></span>|<span data-ttu-id="5653c-141">String</span><span class="sxs-lookup"><span data-stu-id="5653c-141">String</span></span>|<span data-ttu-id="5653c-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5653c-142">Required.</span></span> <span data-ttu-id="5653c-143">Тип создаваемого пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="5653c-143">The type of user flow you are creating.</span></span> <span data-ttu-id="5653c-144">Это значение всегда будет равно `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="5653c-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="5653c-145">усерфловтипеверсион</span><span class="sxs-lookup"><span data-stu-id="5653c-145">userFlowTypeVersion</span></span>|<span data-ttu-id="5653c-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="5653c-146">Float</span></span>|<span data-ttu-id="5653c-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="5653c-147">Required.</span></span> <span data-ttu-id="5653c-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="5653c-148">The version of the user flow.</span></span> <span data-ttu-id="5653c-149">Это значение всегда равно 1.</span><span class="sxs-lookup"><span data-stu-id="5653c-149">This value will always be 1.</span></span>|
|<span data-ttu-id="5653c-150">identityProviders</span><span class="sxs-lookup"><span data-stu-id="5653c-150">identityProviders</span></span>|<span data-ttu-id="5653c-151">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="5653c-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="5653c-152">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="5653c-152">Optional.</span></span> <span data-ttu-id="5653c-153">Поставщики удостоверений, которые необходимо включить в пользовательский блок.</span><span class="sxs-lookup"><span data-stu-id="5653c-153">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="5653c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5653c-154">Response</span></span>

<span data-ttu-id="5653c-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и заголовок Location с URI для объекта [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) , созданного для этого запроса, с `B2X_1` префиксом, добавленным к имени.</span><span class="sxs-lookup"><span data-stu-id="5653c-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="5653c-156">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="5653c-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="5653c-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="5653c-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="5653c-158">Пример 1: создание пользовательского процесса со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="5653c-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="5653c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5653c-159">Request</span></span>

<span data-ttu-id="5653c-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5653c-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5653c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="5653c-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5653c-162">C#</span><span class="sxs-lookup"><span data-stu-id="5653c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5653c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5653c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5653c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5653c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5653c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="5653c-165">Response</span></span>

<span data-ttu-id="5653c-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5653c-166">The following is an example of the response.</span></span>

<span data-ttu-id="5653c-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5653c-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="5653c-168">Пример 2: создание пользовательского процесса со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="5653c-168">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="5653c-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="5653c-169">Request</span></span>

<span data-ttu-id="5653c-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5653c-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5653c-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="5653c-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5653c-172">C#</span><span class="sxs-lookup"><span data-stu-id="5653c-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-b2xuserflow-from-b2xuserflows-identityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5653c-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5653c-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-b2xuserflow-from-b2xuserflows-identityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5653c-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5653c-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-b2xuserflow-from-b2xuserflows-identityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5653c-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="5653c-175">Response</span></span>

<span data-ttu-id="5653c-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5653c-176">The following is an example of the response.</span></span>

<span data-ttu-id="5653c-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5653c-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "Create b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2xUserFlow_from_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


