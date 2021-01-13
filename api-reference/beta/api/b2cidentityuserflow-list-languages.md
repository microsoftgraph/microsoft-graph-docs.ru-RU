---
title: Перечисление языков
description: Получить список языков, поддерживаемых для настройки в пользовательском потоке B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a2fa354f9ab828beeca716fa04472d717f8045a1
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844118"
---
# <a name="list-languages"></a><span data-ttu-id="79987-103">Перечисление языков</span><span class="sxs-lookup"><span data-stu-id="79987-103">List languages</span></span>

<span data-ttu-id="79987-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79987-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79987-105">Получить список языков, поддерживаемых для настройки в пользовательском потоке Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="79987-105">Retrieve a list of languages supported for customization in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="79987-106">**Примечание.** Чтобы получить список языков, поддерживаемых для настройки, необходимо сначала включить настройку языка в пользовательском потоке Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="79987-106">**Note:** To retrieve a list of languages supported for customization, you must first enable language customization on your Azure AD B2C user flow.</span></span> <span data-ttu-id="79987-107">Дополнительные сведения [см. в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="79987-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79987-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79987-108">Permissions</span></span>

<span data-ttu-id="79987-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79987-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79987-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79987-111">Permission type</span></span>      | <span data-ttu-id="79987-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79987-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79987-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79987-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79987-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79987-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="79987-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79987-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="79987-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79987-116">Not supported.</span></span>|
|<span data-ttu-id="79987-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="79987-117">Application</span></span>|<span data-ttu-id="79987-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79987-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="79987-119">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="79987-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="79987-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="79987-120">Global administrator</span></span>
* <span data-ttu-id="79987-121">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="79987-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="79987-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79987-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79987-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79987-123">Optional query parameters</span></span>

<span data-ttu-id="79987-124">Этот метод поддерживает параметр `$filter` запроса для показа только включенных языков.</span><span class="sxs-lookup"><span data-stu-id="79987-124">This method supports the `$filter` query parameter to show only the enabled languages.</span></span> <span data-ttu-id="79987-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="79987-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="79987-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79987-126">Request headers</span></span>

|<span data-ttu-id="79987-127">Имя</span><span class="sxs-lookup"><span data-stu-id="79987-127">Name</span></span>|<span data-ttu-id="79987-128">Описание</span><span class="sxs-lookup"><span data-stu-id="79987-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79987-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79987-129">Authorization</span></span>|<span data-ttu-id="79987-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79987-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79987-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79987-132">Request body</span></span>

<span data-ttu-id="79987-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79987-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79987-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="79987-134">Response</span></span>

<span data-ttu-id="79987-135">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79987-135">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79987-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="79987-136">Examples</span></span>

### <a name="example-1-retrieve-a-list-of-all-languages"></a><span data-ttu-id="79987-137">Пример 1. Извлечение списка всех языков</span><span class="sxs-lookup"><span data-stu-id="79987-137">Example 1: Retrieve a list of all languages</span></span>

#### <a name="request"></a><span data-ttu-id="79987-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="79987-138">Request</span></span>

<span data-ttu-id="79987-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79987-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79987-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="79987-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages
```
# <a name="c"></a>[<span data-ttu-id="79987-141">C#</span><span class="sxs-lookup"><span data-stu-id="79987-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79987-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79987-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79987-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79987-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79987-144">Java</span><span class="sxs-lookup"><span data-stu-id="79987-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79987-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="79987-145">Response</span></span>

<span data-ttu-id="79987-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79987-146">The following is an example of the response.</span></span>

<span data-ttu-id="79987-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="79987-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-retrieve-a-list-of-only-enabled-languages"></a><span data-ttu-id="79987-148">Пример 2. Извлечение списка только включенных языков</span><span class="sxs-lookup"><span data-stu-id="79987-148">Example 2: Retrieve a list of only enabled languages</span></span>

#### <a name="request"></a><span data-ttu-id="79987-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="79987-149">Request</span></span>

<span data-ttu-id="79987-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79987-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79987-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="79987-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_filter"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages?$filter=isEnabled eq true
```
# <a name="c"></a>[<span data-ttu-id="79987-152">C#</span><span class="sxs-lookup"><span data-stu-id="79987-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79987-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79987-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79987-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79987-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79987-155">Java</span><span class="sxs-lookup"><span data-stu-id="79987-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79987-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="79987-156">Response</span></span>

<span data-ttu-id="79987-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79987-157">The following is an example of the response.</span></span>

<span data-ttu-id="79987-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="79987-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
