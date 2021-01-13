---
title: Настройка соединителя API в пользовательском потоке
description: Включив или отключив соединители API для определенного шага в пользовательском потоке, обновив свойство apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 703c1ddd94b5c1de92e606d735b98425c9c99568
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843863"
---
# <a name="configure-userflowapiconnectorconfiguration"></a><span data-ttu-id="49e91-103">Настройка userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="49e91-103">Configure userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="49e91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49e91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49e91-105">Обновите свойство [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) в [потоке b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) чтобы включить или отключить соединители API в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="49e91-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="49e91-106">Каждая связь [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) соответствует определенному шагу в пользовательском потоке, который можно настроить для вызова соединителя API.</span><span class="sxs-lookup"><span data-stu-id="49e91-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="49e91-107">Соединители API настраиваются для определенного шага по одному, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="49e91-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="49e91-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49e91-108">Permissions</span></span>

<span data-ttu-id="49e91-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49e91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49e91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49e91-111">Permission type</span></span>|<span data-ttu-id="49e91-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49e91-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49e91-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49e91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49e91-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49e91-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="49e91-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49e91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49e91-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="49e91-116">Not supported</span></span>|
|<span data-ttu-id="49e91-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="49e91-117">Application</span></span>|<span data-ttu-id="49e91-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49e91-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="49e91-119">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="49e91-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="49e91-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="49e91-120">Global administrator</span></span>
* <span data-ttu-id="49e91-121">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="49e91-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="49e91-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49e91-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{b2xUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="49e91-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49e91-123">Request headers</span></span>

|<span data-ttu-id="49e91-124">Имя</span><span class="sxs-lookup"><span data-stu-id="49e91-124">Name</span></span>|<span data-ttu-id="49e91-125">Описание</span><span class="sxs-lookup"><span data-stu-id="49e91-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="49e91-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49e91-126">Authorization</span></span>|<span data-ttu-id="49e91-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49e91-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="49e91-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49e91-129">Content-Type</span></span>|<span data-ttu-id="49e91-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49e91-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49e91-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49e91-132">Request body</span></span>

<span data-ttu-id="49e91-133">В теле запроса укажите представление идентификатора `id` [IdentityApiConnector](../resources/identityapiconnector.md) в JSON, который вы хотите использовать для конкретного шага.</span><span class="sxs-lookup"><span data-stu-id="49e91-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="49e91-134">Чтобы отключить соединители API, можно использовать значение {} .</span><span class="sxs-lookup"><span data-stu-id="49e91-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="49e91-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e91-135">Response</span></span>

<span data-ttu-id="49e91-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="49e91-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="49e91-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="49e91-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="49e91-138">Пример 1. Enable API connector for Post IDP Federation on sign up</span><span class="sxs-lookup"><span data-stu-id="49e91-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="49e91-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="49e91-139">Request</span></span>

<span data-ttu-id="49e91-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49e91-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="49e91-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="49e91-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="49e91-142">C#</span><span class="sxs-lookup"><span data-stu-id="49e91-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49e91-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49e91-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49e91-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49e91-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49e91-145">Java</span><span class="sxs-lookup"><span data-stu-id="49e91-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="49e91-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e91-146">Response</span></span> 

<span data-ttu-id="49e91-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="49e91-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="49e91-148">Пример 2. Enable API connector for Post Attribute Collection on sign up</span><span class="sxs-lookup"><span data-stu-id="49e91-148">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="49e91-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="49e91-149">Request</span></span> 

<span data-ttu-id="49e91-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49e91-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="49e91-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="49e91-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="49e91-152">C#</span><span class="sxs-lookup"><span data-stu-id="49e91-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49e91-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49e91-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49e91-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49e91-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49e91-155">Java</span><span class="sxs-lookup"><span data-stu-id="49e91-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49e91-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e91-156">Response</span></span>

<span data-ttu-id="49e91-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="49e91-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="49e91-158">Пример 3. Отключение соединители API для коллекции атрибутов Post при регистрации</span><span class="sxs-lookup"><span data-stu-id="49e91-158">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="49e91-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="49e91-159">Request</span></span> 

<span data-ttu-id="49e91-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49e91-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="49e91-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="49e91-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```
# <a name="javascript"></a>[<span data-ttu-id="49e91-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49e91-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49e91-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49e91-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49e91-164">Java</span><span class="sxs-lookup"><span data-stu-id="49e91-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-disable-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49e91-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e91-165">Response</span></span>

<span data-ttu-id="49e91-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="49e91-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
