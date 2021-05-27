---
title: Получить локализованные организационные свойстваBranding
description: Извлечение объекта organizationalbrandingproperties для определенного локального объекта.
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: aaca6728c5c3f3dd94b6a2d27effde1d6d95fba6
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680838"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="b59e8-103">Get Localized organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="b59e8-103">Get Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b59e8-104">Извлечение свойств объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="b59e8-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b59e8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b59e8-105">Permissions</span></span>

<span data-ttu-id="b59e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b59e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b59e8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b59e8-108">Permission type</span></span>                        | <span data-ttu-id="b59e8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b59e8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b59e8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b59e8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b59e8-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="b59e8-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="b59e8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b59e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b59e8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b59e8-113">Not supported.</span></span> |
| <span data-ttu-id="b59e8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b59e8-114">Application</span></span>                            | <span data-ttu-id="b59e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b59e8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b59e8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b59e8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{tenant id}/branding/localizations/{locale}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b59e8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b59e8-117">Optional query parameters</span></span>

<span data-ttu-id="b59e8-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b59e8-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b59e8-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b59e8-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b59e8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b59e8-120">Request headers</span></span>

| <span data-ttu-id="b59e8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b59e8-121">Name</span></span>      |<span data-ttu-id="b59e8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b59e8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b59e8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b59e8-123">Authorization</span></span> | <span data-ttu-id="b59e8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b59e8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b59e8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b59e8-126">Content-Type</span></span>  | <span data-ttu-id="b59e8-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b59e8-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b59e8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b59e8-129">Request body</span></span>

<span data-ttu-id="b59e8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b59e8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b59e8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59e8-131">Response</span></span>

<span data-ttu-id="b59e8-132">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b59e8-132">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="b59e8-133">Значение "id" соответствует запрашиваемой локализации.</span><span class="sxs-lookup"><span data-stu-id="b59e8-133">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="b59e8-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="b59e8-134">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="b59e8-135">Пример 1. Получить локализованный брендинг для определенного локального (fr)</span><span class="sxs-lookup"><span data-stu-id="b59e8-135">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="b59e8-136">Запрос GET для определенной локализации возвращает только значения для этой локализации.</span><span class="sxs-lookup"><span data-stu-id="b59e8-136">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="b59e8-137">Значения Null не будут заменены значениями из брендинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b59e8-137">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="b59e8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b59e8-138">Request</span></span>

<span data-ttu-id="b59e8-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b59e8-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b59e8-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b59e8-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_8"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="b59e8-141">C#</span><span class="sxs-lookup"><span data-stu-id="b59e8-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-8-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b59e8-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b59e8-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-8-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b59e8-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b59e8-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-8-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b59e8-144">Java</span><span class="sxs-lookup"><span data-stu-id="b59e8-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-8-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b59e8-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59e8-145">Response</span></span>

<span data-ttu-id="b59e8-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b59e8-146">The following is an example of the response.</span></span>

> <span data-ttu-id="b59e8-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b59e8-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
"backgroundColor":"#00000F",
"backgroundImage@odata.mediaContentType":"image/*",
"backgroundImage@odata.mediaReadLink": null,
"backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
"bannerLogo@odata.mediaContentType":"image/*",
"bannerLogo@odata.mediaReadLink": null,
"bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
"id":"fr",
"squareLogo@odata.mediaContentType":"image/*",
"squareLogo@odata.mediaReadLink": null,
"squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
"signInPageText":null,
"usernameHintText":null
}
```

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="b59e8-148">Пример 2. Получить все языковые локализации, которые были настроены</span><span class="sxs-lookup"><span data-stu-id="b59e8-148">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="b59e8-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="b59e8-149">Request</span></span>

<span data-ttu-id="b59e8-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b59e8-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b59e8-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="b59e8-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_9"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```
# <a name="c"></a>[<span data-ttu-id="b59e8-152">C#</span><span class="sxs-lookup"><span data-stu-id="b59e8-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-9-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b59e8-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b59e8-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-9-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b59e8-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b59e8-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-9-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b59e8-155">Java</span><span class="sxs-lookup"><span data-stu-id="b59e8-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-9-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b59e8-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59e8-156">Response</span></span>

<span data-ttu-id="b59e8-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b59e8-157">The following is an example of the response.</span></span>

> <span data-ttu-id="b59e8-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b59e8-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
 "values": [
   {
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "backgroundImage@odata.mediaEditLink":"https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id":"en-us",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
   },
   {
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id":"fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":null,
    "usernameHintText":null
   }
 ]
}
```

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="b59e8-159">Пример 3. Получить значение signInPageText для определенного локального значения</span><span class="sxs-lookup"><span data-stu-id="b59e8-159">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="b59e8-160">Запрос свойства локализации возвращает это значение или 204, если значение null.</span><span class="sxs-lookup"><span data-stu-id="b59e8-160">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="b59e8-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="b59e8-161">Request</span></span>

<span data-ttu-id="b59e8-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b59e8-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b59e8-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="b59e8-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_10"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```
# <a name="c"></a>[<span data-ttu-id="b59e8-164">C#</span><span class="sxs-lookup"><span data-stu-id="b59e8-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-10-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b59e8-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b59e8-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-10-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b59e8-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b59e8-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-10-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b59e8-167">Java</span><span class="sxs-lookup"><span data-stu-id="b59e8-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-10-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b59e8-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="b59e8-168">Response</span></span>

<span data-ttu-id="b59e8-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b59e8-169">The following is an example of the response.</span></span>

> <span data-ttu-id="b59e8-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b59e8-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
"value":"Welcome"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
