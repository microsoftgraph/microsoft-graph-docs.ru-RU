---
title: Перечисление языков
description: Извлечение списка языков, поддерживаемых для настройки в потоке пользователей B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e3b04b25796b7864d6dda74eaa7b2edc14b30c93
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438297"
---
# <a name="list-languages"></a><span data-ttu-id="fc809-103">Перечисление языков</span><span class="sxs-lookup"><span data-stu-id="fc809-103">List languages</span></span>

<span data-ttu-id="fc809-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc809-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc809-105">Извлечение списка языков, поддерживаемых для настройки в потоке пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="fc809-105">Retrieve a list of languages supported for customization in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="fc809-106">**Примечание:** Чтобы получить список языков, поддерживаемых для настройки, сначала необходимо включить настройку языка в потоке пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="fc809-106">**Note:** To retrieve a list of languages supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="fc809-107">Дополнительные сведения см. [в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="fc809-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc809-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc809-108">Permissions</span></span>

<span data-ttu-id="fc809-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc809-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc809-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc809-111">Permission type</span></span>      | <span data-ttu-id="fc809-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc809-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc809-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc809-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc809-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc809-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fc809-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc809-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fc809-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc809-116">Not supported.</span></span>|
|<span data-ttu-id="fc809-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fc809-117">Application</span></span>|<span data-ttu-id="fc809-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc809-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fc809-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="fc809-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fc809-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="fc809-120">Global administrator</span></span>
* <span data-ttu-id="fc809-121">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="fc809-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fc809-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc809-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc809-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc809-123">Optional query parameters</span></span>

<span data-ttu-id="fc809-124">Этот метод поддерживает параметр `$filter` запроса, чтобы показывать только языки с включенной поддержкой.</span><span class="sxs-lookup"><span data-stu-id="fc809-124">This method supports the `$filter` query parameter to show only the enabled languages.</span></span> <span data-ttu-id="fc809-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fc809-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc809-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc809-126">Request headers</span></span>

|<span data-ttu-id="fc809-127">Имя</span><span class="sxs-lookup"><span data-stu-id="fc809-127">Name</span></span>|<span data-ttu-id="fc809-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fc809-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fc809-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc809-129">Authorization</span></span>|<span data-ttu-id="fc809-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc809-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc809-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc809-132">Request body</span></span>

<span data-ttu-id="fc809-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc809-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc809-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc809-134">Response</span></span>

<span data-ttu-id="fc809-135">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fc809-135">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc809-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="fc809-136">Examples</span></span>

### <a name="example-1-retrieve-a-list-of-all-languages"></a><span data-ttu-id="fc809-137">Пример 1. Извлечение списка всех языков</span><span class="sxs-lookup"><span data-stu-id="fc809-137">Example 1: Retrieve a list of all languages</span></span>

#### <a name="request"></a><span data-ttu-id="fc809-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc809-138">Request</span></span>

<span data-ttu-id="fc809-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc809-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fc809-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc809-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages
```
# <a name="c"></a>[<span data-ttu-id="fc809-141">C#</span><span class="sxs-lookup"><span data-stu-id="fc809-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc809-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc809-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc809-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc809-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc809-144">Java</span><span class="sxs-lookup"><span data-stu-id="fc809-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc809-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc809-145">Response</span></span>

<span data-ttu-id="fc809-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc809-146">The following is an example of the response.</span></span>

<span data-ttu-id="fc809-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fc809-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": false,
      "displayName": "Deutsch"
    }
  ]
}
```

### <a name="example-2-retrieve-a-list-of-only-enabled-languages"></a><span data-ttu-id="fc809-148">Пример 2. Извлечение списка только включенных языков</span><span class="sxs-lookup"><span data-stu-id="fc809-148">Example 2: Retrieve a list of only enabled languages</span></span>

#### <a name="request"></a><span data-ttu-id="fc809-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc809-149">Request</span></span>

<span data-ttu-id="fc809-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc809-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fc809-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc809-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_filter"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages?$filter=isEnabled eq true
```
# <a name="c"></a>[<span data-ttu-id="fc809-152">C#</span><span class="sxs-lookup"><span data-stu-id="fc809-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc809-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc809-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc809-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc809-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc809-155">Java</span><span class="sxs-lookup"><span data-stu-id="fc809-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc809-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc809-156">Response</span></span>

<span data-ttu-id="fc809-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc809-157">The following is an example of the response.</span></span>

<span data-ttu-id="fc809-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fc809-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    }
  ]
}
```
