---
title: Обновление apiConnectorКонфигурация
description: Включить или отключить разъем API на определенном этапе пользовательского потока путем обновления свойства apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e1c223bbe7fa16800cc7b4bedc07ea3129a0b3cd
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547108"
---
# <a name="update-apiconnectorconfiguration"></a><span data-ttu-id="7c67b-103">Обновление apiConnectorКонфигурация</span><span class="sxs-lookup"><span data-stu-id="7c67b-103">Update apiConnectorConfiguration</span></span>

<span data-ttu-id="7c67b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c67b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c67b-105">Обновление свойства [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) в [b2xIdentityUserFlow для](../resources/b2xidentityuserflow.md) включения или отключения разъема API в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="7c67b-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="7c67b-106">Каждое отношение [apiConnectorConfiguration соответствует](../resources/userflowapiconnectorconfiguration.md) определенному шагу в пользовательском потоке, который может быть настроен для вызова разъема API.</span><span class="sxs-lookup"><span data-stu-id="7c67b-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="7c67b-107">Настраиваете разъем API для определенного шага по одному, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="7c67b-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c67b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c67b-108">Permissions</span></span>

<span data-ttu-id="7c67b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c67b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c67b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c67b-111">Permission type</span></span>|<span data-ttu-id="7c67b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c67b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c67b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c67b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c67b-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c67b-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7c67b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c67b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c67b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7c67b-116">Not supported</span></span>|
|<span data-ttu-id="7c67b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7c67b-117">Application</span></span>|<span data-ttu-id="7c67b-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c67b-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7c67b-119">Рабочий или школьный счет должен принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="7c67b-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7c67b-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7c67b-120">Global administrator</span></span>
* <span data-ttu-id="7c67b-121">Администратор внешней идентификации Flow пользователя</span><span class="sxs-lookup"><span data-stu-id="7c67b-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7c67b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c67b-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{b2xUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7c67b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c67b-123">Request headers</span></span>

|<span data-ttu-id="7c67b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="7c67b-124">Name</span></span>|<span data-ttu-id="7c67b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7c67b-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7c67b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c67b-126">Authorization</span></span>|<span data-ttu-id="7c67b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c67b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7c67b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c67b-129">Content-Type</span></span>|<span data-ttu-id="7c67b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c67b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c67b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c67b-132">Request body</span></span>

<span data-ttu-id="7c67b-133">В органе запроса предоставьте представление JSON удостоверения `id` [ApiConnector, который](../resources/identityapiconnector.md) вы хотите использовать на определенном этапе.</span><span class="sxs-lookup"><span data-stu-id="7c67b-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="7c67b-134">Чтобы отключить разъем API, значение может {} быть.</span><span class="sxs-lookup"><span data-stu-id="7c67b-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="7c67b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c67b-135">Response</span></span>

<span data-ttu-id="7c67b-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7c67b-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7c67b-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="7c67b-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="7c67b-138">Пример 1: Включить разъем API для Почтовой Федерации ВПЛ при регистрации</span><span class="sxs-lookup"><span data-stu-id="7c67b-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="7c67b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c67b-139">Request</span></span>

<span data-ttu-id="7c67b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c67b-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7c67b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c67b-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="7c67b-142">C#</span><span class="sxs-lookup"><span data-stu-id="7c67b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c67b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c67b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c67b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c67b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c67b-145">Java</span><span class="sxs-lookup"><span data-stu-id="7c67b-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-postfederationsignup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7c67b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c67b-146">Response</span></span> 

<span data-ttu-id="7c67b-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7c67b-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="7c67b-148">Пример 2: Включить разъем API для коллекции почтовых атрибутов при регистрации</span><span class="sxs-lookup"><span data-stu-id="7c67b-148">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="7c67b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c67b-149">Request</span></span> 

<span data-ttu-id="7c67b-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c67b-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7c67b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c67b-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"   
}
```
# <a name="c"></a>[<span data-ttu-id="7c67b-152">C#</span><span class="sxs-lookup"><span data-stu-id="7c67b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c67b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c67b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c67b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c67b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c67b-155">Java</span><span class="sxs-lookup"><span data-stu-id="7c67b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-b2xuserflows-apiconnectorconfiguration-postattributecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7c67b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c67b-156">Response</span></span>

<span data-ttu-id="7c67b-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7c67b-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="7c67b-158">Пример 3: Отключить разъем API для коллекции почтовых атрибутов при регистрации</span><span class="sxs-lookup"><span data-stu-id="7c67b-158">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="7c67b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c67b-159">Request</span></span> 

<span data-ttu-id="7c67b-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c67b-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```


#### <a name="response"></a><span data-ttu-id="7c67b-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c67b-161">Response</span></span>

<span data-ttu-id="7c67b-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7c67b-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
