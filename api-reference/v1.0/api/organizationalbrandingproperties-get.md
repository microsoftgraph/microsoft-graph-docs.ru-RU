---
title: Get organizationalBrandingProperties
description: Извлечение свойств и связей объекта organizationalBrandingProperties.
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 52fab233f7f84636b1daf3fc7535608beb9267b1
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682504"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="7b52f-103">Get organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="7b52f-103">Get organizationalBrandingProperties</span></span>

<span data-ttu-id="7b52f-104">Извлечение свойств и связей объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="7b52f-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b52f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b52f-105">Permissions</span></span>

<span data-ttu-id="7b52f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b52f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b52f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b52f-108">Permission type</span></span>                        | <span data-ttu-id="7b52f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b52f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b52f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b52f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b52f-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="7b52f-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="7b52f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b52f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b52f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b52f-113">Not supported.</span></span> |
| <span data-ttu-id="7b52f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b52f-114">Application</span></span>                            | <span data-ttu-id="7b52f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b52f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b52f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b52f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{tenant id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="7b52f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b52f-117">Request headers</span></span>

| <span data-ttu-id="7b52f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7b52f-118">Name</span></span>      |<span data-ttu-id="7b52f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7b52f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b52f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b52f-120">Authorization</span></span> | <span data-ttu-id="7b52f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b52f-p102">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="7b52f-123">При попытке запроса в Graph Explorer необходимо также включить заглавную головку запроса **Accept-Language** с допустимым локализом ISO-639.</span><span class="sxs-lookup"><span data-stu-id="7b52f-123">If you try the query in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="7b52f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b52f-124">Request body</span></span>

<span data-ttu-id="7b52f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b52f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b52f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b52f-126">Response</span></span>

<span data-ttu-id="7b52f-127">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7b52f-127">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7b52f-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7b52f-128">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="7b52f-129">Пример 1. Получить брендинг по умолчанию</span><span class="sxs-lookup"><span data-stu-id="7b52f-129">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="7b52f-130">Если вы попробуете пример в Graph Explorer, необходимо также включить заглавную головку запроса **Accept-Language** с допустимым локальным кодом ISO-639, чтобы избежать ошибки " Значение недействительный код местного значения *en-US,en;q=0.9. Это должен быть допустимый локал ISO-639.*</span><span class="sxs-lookup"><span data-stu-id="7b52f-130">If you try the example in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale to avoid getting an error "*Invalid locale id value en-US,en;q=0.9. It must be a valid ISO-639 locale.*"</span></span>

#### <a name="request"></a><span data-ttu-id="7b52f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b52f-131">Request</span></span>

<span data-ttu-id="7b52f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b52f-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b52f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b52f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="7b52f-134">C#</span><span class="sxs-lookup"><span data-stu-id="7b52f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b52f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b52f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b52f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b52f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b52f-137">Java</span><span class="sxs-lookup"><span data-stu-id="7b52f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b52f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b52f-138">Response</span></span>

<span data-ttu-id="7b52f-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b52f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="7b52f-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7b52f-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "bannerLogo@odata.mediaContentType":"image/*",
  "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "id": "und",
  "squareLogo@odata.mediaContentType":"image/*",
  "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "signInPageText":"Default",
  "usernameHintText":"DefaultHint"
}
```

<span data-ttu-id="7b52f-141">Запросы на /branding всегда возвращают **свойства mediaContentType,** **mediaReadLink** и **mediaEditLink.**</span><span class="sxs-lookup"><span data-stu-id="7b52f-141">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="7b52f-142">Если был применен локализ, **mediaEditLink** — это **mediaEditLink** для локального (который всегда не является null), а **mediaReadLink** и **mediaContentType** — **это mediaReadLink** и **mediaContentType** локального сайта, если **mediaReadLink** локального сайта не является null; в противном случае **по умолчанию mediaReadLink** и **mediaContentType**.</span><span class="sxs-lookup"><span data-stu-id="7b52f-142">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="7b52f-143">Пример 2. Получить организационный брендинг, но не настроить брендинг</span><span class="sxs-lookup"><span data-stu-id="7b52f-143">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="7b52f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b52f-144">Request</span></span>

<span data-ttu-id="7b52f-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b52f-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="7b52f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b52f-146">Response</span></span>

<span data-ttu-id="7b52f-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b52f-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="7b52f-148">Пример 3. Получить организационный брендинг для французского языка</span><span class="sxs-lookup"><span data-stu-id="7b52f-148">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="7b52f-149">**Заготвка Accept-Language** используется для применения определенной локализации к брендингу.</span><span class="sxs-lookup"><span data-stu-id="7b52f-149">The **Accept-Language** header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="7b52f-150">Свойства, `null` указанные в указанной локализации, возвращаются из фирменого бренда по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7b52f-150">Properties that are `null` in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="7b52f-151">Если в **запросе указан** заглавный загон Accept-Language, ответ будет включать заглавный загон **Content-Language,** если это не `und` так.</span><span class="sxs-lookup"><span data-stu-id="7b52f-151">If the **Accept-Language** header is specified in the request, the response will include the **Content-Language** header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="7b52f-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b52f-152">Request</span></span>

<span data-ttu-id="7b52f-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b52f-153">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="7b52f-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b52f-154">Response</span></span>

<span data-ttu-id="7b52f-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b52f-155">The following is an example of the response.</span></span>

> <span data-ttu-id="7b52f-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7b52f-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "und",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="7b52f-157">Пример 4. Получить bannerLogo для французского языка</span><span class="sxs-lookup"><span data-stu-id="7b52f-157">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="7b52f-158">Возвращает **bannerLogo** для `fr` локального, если он существует.</span><span class="sxs-lookup"><span data-stu-id="7b52f-158">Returns **bannerLogo** for the `fr` locale if it exists.</span></span> <span data-ttu-id="7b52f-159">Если локализация не существует, возвращается **баннер по умолчаниюLogo**.</span><span class="sxs-lookup"><span data-stu-id="7b52f-159">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="7b52f-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b52f-160">Request</span></span>

<span data-ttu-id="7b52f-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b52f-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7b52f-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b52f-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_5"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```
# <a name="c"></a>[<span data-ttu-id="7b52f-163">C#</span><span class="sxs-lookup"><span data-stu-id="7b52f-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b52f-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b52f-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b52f-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b52f-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b52f-166">Java</span><span class="sxs-lookup"><span data-stu-id="7b52f-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b52f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b52f-167">Response</span></span>

<span data-ttu-id="7b52f-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b52f-168">The following is an example of the response.</span></span>

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
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
}
```

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="7b52f-169">Пример 5. Получить bannerLogo, когда не настроен bannerLogo</span><span class="sxs-lookup"><span data-stu-id="7b52f-169">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="7b52f-170">В этом примере показан запрос на свойство, которое не существует в фирменой марке по умолчанию или на языке, указанном в загородной головке **Accept-Language.**</span><span class="sxs-lookup"><span data-stu-id="7b52f-170">This example shows a request for a property that does not exist on the default branding or the language specified in the **Accept-Language** header.</span></span>

#### <a name="request"></a><span data-ttu-id="7b52f-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b52f-171">Request</span></span>

<span data-ttu-id="7b52f-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b52f-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b52f-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b52f-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_6"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```
# <a name="c"></a>[<span data-ttu-id="7b52f-174">C#</span><span class="sxs-lookup"><span data-stu-id="7b52f-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b52f-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b52f-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b52f-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b52f-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b52f-177">Java</span><span class="sxs-lookup"><span data-stu-id="7b52f-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b52f-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b52f-178">Response</span></span>

<span data-ttu-id="7b52f-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b52f-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
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
