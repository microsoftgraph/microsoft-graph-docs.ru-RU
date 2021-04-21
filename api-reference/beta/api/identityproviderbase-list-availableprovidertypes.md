---
title: Список доступныхProviderTypes
description: Извлечение всех доступных типов поставщика удостоверений в каталоге.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3282ed8aff91e6fe82d62593be13efa052248abc
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921423"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="28825-103">Список доступныхProviderTypes</span><span class="sxs-lookup"><span data-stu-id="28825-103">List availableProviderTypes</span></span>

<span data-ttu-id="28825-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28825-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28825-105">Извлекает все типы поставщиков удостоверений, доступные в каталоге.</span><span class="sxs-lookup"><span data-stu-id="28825-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="28825-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28825-106">Permissions</span></span>

<span data-ttu-id="28825-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28825-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28825-109">Permission type</span></span>      | <span data-ttu-id="28825-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28825-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28825-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28825-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28825-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28825-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="28825-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28825-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="28825-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28825-114">Not supported.</span></span>|
|<span data-ttu-id="28825-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="28825-115">Application</span></span>|<span data-ttu-id="28825-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28825-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="28825-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="28825-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="28825-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="28825-118">Global Administrator</span></span>
* <span data-ttu-id="28825-119">Администратор внешнего поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="28825-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="28825-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28825-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="28825-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28825-121">Request headers</span></span>

|<span data-ttu-id="28825-122">Имя</span><span class="sxs-lookup"><span data-stu-id="28825-122">Name</span></span>|<span data-ttu-id="28825-123">Описание</span><span class="sxs-lookup"><span data-stu-id="28825-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="28825-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28825-124">Authorization</span></span>|<span data-ttu-id="28825-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28825-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28825-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28825-127">Request body</span></span>
<span data-ttu-id="28825-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28825-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28825-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="28825-129">Response</span></span>

<span data-ttu-id="28825-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28825-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28825-131">Пример</span><span class="sxs-lookup"><span data-stu-id="28825-131">Example</span></span>

### <a name="example-1-list-all-identityprovider-available-in-an-azure-ad-directory"></a><span data-ttu-id="28825-132">Пример 1. Список всех **identityProvider,** доступных в каталоге Azure AD</span><span class="sxs-lookup"><span data-stu-id="28825-132">Example 1: List all **identityProvider** available in an Azure AD directory</span></span>

### <a name="request"></a><span data-ttu-id="28825-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="28825-133">Request</span></span>
<span data-ttu-id="28825-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28825-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28825-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="28825-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="28825-136">C#</span><span class="sxs-lookup"><span data-stu-id="28825-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28825-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28825-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28825-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28825-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28825-139">Java</span><span class="sxs-lookup"><span data-stu-id="28825-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="28825-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="28825-140">Response</span></span>

<span data-ttu-id="28825-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28825-141">The following is an example of the response.</span></span>

<span data-ttu-id="28825-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="28825-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "MicrosoftAccount",
        "EmailOTP",
        "Facebook",
        "Google"
    ]
}
```

### <a name="example-2-list-all-identityprovider-available-in-an-azure-ad-b2c-directory"></a><span data-ttu-id="28825-143">Пример 2. Список всех **identityProvider,** доступных в каталоге Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="28825-143">Example 2: List all **identityProvider** available in an Azure AD B2C directory</span></span>

### <a name="request"></a><span data-ttu-id="28825-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="28825-144">Request</span></span>
<span data-ttu-id="28825-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28825-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28825-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="28825-146">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="28825-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="28825-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes_b2c"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="28825-148">C#</span><span class="sxs-lookup"><span data-stu-id="28825-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-b2c-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28825-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28825-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-b2c-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28825-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28825-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-b2c-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28825-151">Java</span><span class="sxs-lookup"><span data-stu-id="28825-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-b2c-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="28825-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="28825-152">Response</span></span>

<span data-ttu-id="28825-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28825-153">The following is an example of the response.</span></span>

<span data-ttu-id="28825-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="28825-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
 "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
  "value": [
        "Microsoft",
        "Google",
        "Facebook",
        "Amazon",
        "LinkedIn",
        "Weibo",
        "QQ",
        "WeChat",
        "Twitter",
        "GitHub",
        "AppleManaged",
        "OpenIdConnect"
  ]
}
```
