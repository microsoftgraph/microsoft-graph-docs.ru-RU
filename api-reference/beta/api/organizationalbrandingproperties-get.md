---
title: Get organizationalBrandingProperties
description: Извлечение свойств и связей объекта organizationalBrandingProperties.
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bdc652c7e6a2238bb0061e342c181cd9575ab45c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785934"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="4b98e-103">Get organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="4b98e-103">Get organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b98e-104">Извлечение свойств и связей объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="4b98e-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b98e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b98e-105">Permissions</span></span>

<span data-ttu-id="4b98e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b98e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b98e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b98e-108">Permission type</span></span>                        | <span data-ttu-id="4b98e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b98e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b98e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b98e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b98e-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4b98e-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="4b98e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b98e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b98e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b98e-113">Not supported.</span></span> |
| <span data-ttu-id="4b98e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b98e-114">Application</span></span>                            | <span data-ttu-id="4b98e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b98e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b98e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b98e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{tenant id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b98e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4b98e-117">Optional query parameters</span></span>

<span data-ttu-id="4b98e-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4b98e-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4b98e-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4b98e-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b98e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b98e-120">Request headers</span></span>

| <span data-ttu-id="4b98e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4b98e-121">Name</span></span>      |<span data-ttu-id="4b98e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4b98e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4b98e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b98e-123">Authorization</span></span> | <span data-ttu-id="4b98e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b98e-p103">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="4b98e-126">При попытке запроса в Graph Explorer необходимо также включить Accept-Language запроса с допустимым локализом ISO-639.</span><span class="sxs-lookup"><span data-stu-id="4b98e-126">If you try the query in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="4b98e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b98e-127">Request body</span></span>

<span data-ttu-id="4b98e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b98e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b98e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b98e-129">Response</span></span>

<span data-ttu-id="4b98e-130">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4b98e-130">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b98e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4b98e-131">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="4b98e-132">Пример 1. Получить брендинг по умолчанию</span><span class="sxs-lookup"><span data-stu-id="4b98e-132">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="4b98e-133">Если вы попробуете пример в Graph Explorer, необходимо также включить Accept-Language запроса с допустимым локальным кодом ISO-639, чтобы избежать ошибки "Недействительное значение id locale en-US,en;q=0.9.</span><span class="sxs-lookup"><span data-stu-id="4b98e-133">If you try the example in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale to avoid getting an error "Invalid locale id value en-US,en;q=0.9.</span></span> <span data-ttu-id="4b98e-134">Это должен быть допустимый локал ISO-639".</span><span class="sxs-lookup"><span data-stu-id="4b98e-134">It must be a valid ISO-639 locale."</span></span>

#### <a name="request"></a><span data-ttu-id="4b98e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b98e-135">Request</span></span>

<span data-ttu-id="4b98e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b98e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b98e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b98e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="4b98e-138">C#</span><span class="sxs-lookup"><span data-stu-id="4b98e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b98e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b98e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b98e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b98e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b98e-141">Java</span><span class="sxs-lookup"><span data-stu-id="4b98e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b98e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b98e-142">Response</span></span>

<span data-ttu-id="4b98e-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b98e-143">The following is an example of the response.</span></span>

> <span data-ttu-id="4b98e-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4b98e-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "backgroundColor":"#FFFF33",
  "backgroundImage@odata.mediaContentType":"image/*",
  "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "bannerLogo@odata.mediaContentType":"image/*",
  "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "id": "und",
  "squareLogo@odata.mediaContentType":"image/*",
  "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "signInPageText":"Default",
  "usernameHintText":"DefaultHint"
}
```

<span data-ttu-id="4b98e-145">Запросы на /branding всегда возвращают **свойства mediaContentType,** **mediaReadLink** и **mediaEditLink.**</span><span class="sxs-lookup"><span data-stu-id="4b98e-145">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="4b98e-146">Если был применен локализ, **mediaEditLink** — это **mediaEditLink** для локального (который всегда не является null), а **mediaReadLink** и **mediaContentType** — **это mediaReadLink** и **mediaContentType** локального сайта, если **mediaReadLink** локального сайта не является null; в противном случае **по умолчанию mediaReadLink** и **mediaContentType**.</span><span class="sxs-lookup"><span data-stu-id="4b98e-146">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="4b98e-147">Пример 2. Получить организационный брендинг, но не настроить брендинг</span><span class="sxs-lookup"><span data-stu-id="4b98e-147">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="4b98e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b98e-148">Request</span></span>

<span data-ttu-id="4b98e-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b98e-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="4b98e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b98e-150">Response</span></span>

<span data-ttu-id="4b98e-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b98e-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="4b98e-152">Пример 3. Получить организационный брендинг для французского языка</span><span class="sxs-lookup"><span data-stu-id="4b98e-152">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="4b98e-153">Заго Accept-Langauge используется для применения определенной локализации к брендингу.</span><span class="sxs-lookup"><span data-stu-id="4b98e-153">The Accept-Langauge header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="4b98e-154">Свойства, которые являются недействительными в указанной локализации, возвращаются из брендинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4b98e-154">Properties that are null in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="4b98e-155">Если Accept-Language в запросе указана загонщика, ответ будет включать заглавный заглавный контент-язык, если это не `und` так.</span><span class="sxs-lookup"><span data-stu-id="4b98e-155">If the Accept-Language header is specified in the request, the response will include the Content-Language header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="4b98e-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b98e-156">Request</span></span>

<span data-ttu-id="4b98e-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b98e-157">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="4b98e-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b98e-158">Response</span></span>

<span data-ttu-id="4b98e-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b98e-159">The following is an example of the response.</span></span>

> <span data-ttu-id="4b98e-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4b98e-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "und",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="4b98e-161">Пример 4. Получить bannerLogo для французского языка</span><span class="sxs-lookup"><span data-stu-id="4b98e-161">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="4b98e-162">Возвращает **bannerLogo** для fr locale, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4b98e-162">Returns **bannerLogo** for the fr locale if it exists.</span></span> <span data-ttu-id="4b98e-163">Если локализация не существует, возвращается **баннер по умолчаниюLogo**.</span><span class="sxs-lookup"><span data-stu-id="4b98e-163">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="4b98e-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b98e-164">Request</span></span>

<span data-ttu-id="4b98e-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b98e-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b98e-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b98e-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_5"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```
# <a name="c"></a>[<span data-ttu-id="4b98e-167">C#</span><span class="sxs-lookup"><span data-stu-id="4b98e-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b98e-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b98e-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b98e-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b98e-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b98e-170">Java</span><span class="sxs-lookup"><span data-stu-id="4b98e-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b98e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b98e-171">Response</span></span>

<span data-ttu-id="4b98e-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b98e-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
}
```

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="4b98e-173">Пример 5. Получить bannerLogo, когда не настроен bannerLogo</span><span class="sxs-lookup"><span data-stu-id="4b98e-173">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="4b98e-174">В этом примере показан запрос на свойство, которое не существует в фирменой марке по умолчанию или языка, указанного в Accept-Language.</span><span class="sxs-lookup"><span data-stu-id="4b98e-174">This example shows a request for a property that does not exist on the default branding or the language specified in the Accept-Language header.</span></span>

#### <a name="request"></a><span data-ttu-id="4b98e-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b98e-175">Request</span></span>

<span data-ttu-id="4b98e-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b98e-176">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b98e-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b98e-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_6"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```
# <a name="c"></a>[<span data-ttu-id="4b98e-178">C#</span><span class="sxs-lookup"><span data-stu-id="4b98e-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b98e-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b98e-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b98e-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b98e-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b98e-181">Java</span><span class="sxs-lookup"><span data-stu-id="4b98e-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b98e-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b98e-182">Response</span></span>

<span data-ttu-id="4b98e-183">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b98e-183">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 NO CONTENT
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
