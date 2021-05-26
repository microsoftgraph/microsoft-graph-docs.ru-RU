---
title: Настройка соединителя API в пользовательском потоке
description: Включить или отключить соединители API для определенного шага в потоке пользователей, обновив свойство apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d20c8674eac53713540efd42b18da22cc929a6a8
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664502"
---
# <a name="configure-userflowapiconnectorconfiguration"></a><span data-ttu-id="9ae29-103">Настройка userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ae29-103">Configure userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="9ae29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ae29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ae29-105">[Обнови свойство apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) в [потоке b2cIdentityUserFlow,](../resources/b2cidentityuserflow.md) чтобы включить или отключить соединителю API в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="9ae29-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="9ae29-106">Каждое отношение [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) соответствует определенному шагу в потоке пользователей, который можно настроить для вызова соединителя API.</span><span class="sxs-lookup"><span data-stu-id="9ae29-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="9ae29-107">Вы настраивает соединители API для определенного шага одновременно, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="9ae29-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ae29-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ae29-108">Permissions</span></span>

<span data-ttu-id="9ae29-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ae29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ae29-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ae29-111">Permission type</span></span>|<span data-ttu-id="9ae29-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ae29-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ae29-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ae29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ae29-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ae29-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9ae29-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ae29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ae29-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9ae29-116">Not supported</span></span>|
|<span data-ttu-id="9ae29-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ae29-117">Application</span></span>|<span data-ttu-id="9ae29-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ae29-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9ae29-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="9ae29-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9ae29-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9ae29-120">Global administrator</span></span>
* <span data-ttu-id="9ae29-121">Администратор внешних Flow удостоверений</span><span class="sxs-lookup"><span data-stu-id="9ae29-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9ae29-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ae29-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{b2cUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9ae29-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ae29-123">Request headers</span></span>

|<span data-ttu-id="9ae29-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9ae29-124">Name</span></span>|<span data-ttu-id="9ae29-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9ae29-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9ae29-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ae29-126">Authorization</span></span>|<span data-ttu-id="9ae29-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ae29-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9ae29-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ae29-129">Content-Type</span></span>|<span data-ttu-id="9ae29-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ae29-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ae29-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ae29-132">Request body</span></span>

<span data-ttu-id="9ae29-133">В теле запроса уделяем JSON представление `id` [удостоверенияApiConnector,](../resources/identityapiconnector.md) который необходимо использовать для определенного шага.</span><span class="sxs-lookup"><span data-stu-id="9ae29-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="9ae29-134">Чтобы отключить соединители API, значение может быть {} .</span><span class="sxs-lookup"><span data-stu-id="9ae29-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="9ae29-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ae29-135">Response</span></span>

<span data-ttu-id="9ae29-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9ae29-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9ae29-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ae29-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="9ae29-138">Пример 1. Включить соединители API для Федерации почтовых IDP при регистрации</span><span class="sxs-lookup"><span data-stu-id="9ae29-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="9ae29-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ae29-139">Request</span></span>

<span data-ttu-id="9ae29-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ae29-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ae29-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ae29-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="9ae29-142">C#</span><span class="sxs-lookup"><span data-stu-id="9ae29-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ae29-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ae29-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ae29-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ae29-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ae29-145">Java</span><span class="sxs-lookup"><span data-stu-id="9ae29-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-postfederationsignup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="9ae29-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ae29-146">Response</span></span> 

<span data-ttu-id="9ae29-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ae29-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="9ae29-148">Пример 2. Включить соединители API для коллекции атрибутов post при регистрации</span><span class="sxs-lookup"><span data-stu-id="9ae29-148">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="9ae29-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ae29-149">Request</span></span> 

<span data-ttu-id="9ae29-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ae29-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ae29-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ae29-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="9ae29-152">C#</span><span class="sxs-lookup"><span data-stu-id="9ae29-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ae29-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ae29-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ae29-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ae29-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ae29-155">Java</span><span class="sxs-lookup"><span data-stu-id="9ae29-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ae29-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ae29-156">Response</span></span>

<span data-ttu-id="9ae29-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ae29-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="9ae29-158">Пример 3. Отключение соединители API для коллекции атрибутов post при регистрации</span><span class="sxs-lookup"><span data-stu-id="9ae29-158">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="9ae29-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ae29-159">Request</span></span> 

<span data-ttu-id="9ae29-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ae29-160">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="9ae29-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ae29-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2cuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```
# <a name="javascript"></a>[<span data-ttu-id="9ae29-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ae29-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ae29-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ae29-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ae29-164">Java</span><span class="sxs-lookup"><span data-stu-id="9ae29-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2cuserflows-apiconnectorconfiguration-disable-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ae29-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ae29-165">Response</span></span>

<span data-ttu-id="9ae29-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9ae29-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
