---
title: Get organizationalBrandingProperties
description: Извлечение свойств и связей объекта organizationalBrandingProperties.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: aa41c0d9e8e31f1cbe7a4c4653a27168c67a1a2c
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582818"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="3f8ef-103">Get organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="3f8ef-103">Get organizationalBrandingProperties</span></span>

<span data-ttu-id="3f8ef-104">Извлечение свойств и связей объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="3f8ef-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f8ef-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f8ef-105">Permissions</span></span>

<span data-ttu-id="3f8ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f8ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f8ef-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f8ef-108">Permission type</span></span>                        | <span data-ttu-id="3f8ef-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f8ef-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3f8ef-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f8ef-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f8ef-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="3f8ef-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="3f8ef-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f8ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f8ef-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-113">Not supported.</span></span> |
| <span data-ttu-id="3f8ef-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f8ef-114">Application</span></span>                            | <span data-ttu-id="3f8ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f8ef-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f8ef-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="3f8ef-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f8ef-117">Request headers</span></span>

| <span data-ttu-id="3f8ef-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3f8ef-118">Name</span></span>      |<span data-ttu-id="3f8ef-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3f8ef-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3f8ef-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f8ef-120">Authorization</span></span> | <span data-ttu-id="3f8ef-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-p102">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="3f8ef-123">При попытке запроса в Graph Explorer необходимо также включить заглавную головку запроса **Accept-Language** с допустимым локализом ISO-639.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-123">If you try the query in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="3f8ef-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f8ef-124">Request body</span></span>

<span data-ttu-id="3f8ef-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f8ef-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f8ef-126">Response</span></span>

<span data-ttu-id="3f8ef-127">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-127">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f8ef-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3f8ef-128">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="3f8ef-129">Пример 1. Получить брендинг по умолчанию</span><span class="sxs-lookup"><span data-stu-id="3f8ef-129">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="3f8ef-130">Если вы попробуете пример в Graph Explorer, необходимо также включить заглавную головку запроса **Accept-Language** с допустимым локальным кодом ISO-639, чтобы избежать ошибки " Значение недействительный код локального языка *en-US,en;q=0.9. Это должен быть допустимый локал ISO-639.*</span><span class="sxs-lookup"><span data-stu-id="3f8ef-130">If you try the example in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale to avoid getting an error "*Invalid locale id value en-US,en;q=0.9. It must be a valid ISO-639 locale.*"</span></span>

#### <a name="request"></a><span data-ttu-id="3f8ef-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f8ef-131">Request</span></span>

<span data-ttu-id="3f8ef-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f8ef-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f8ef-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="3f8ef-134">C#</span><span class="sxs-lookup"><span data-stu-id="3f8ef-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f8ef-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f8ef-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f8ef-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f8ef-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f8ef-137">Java</span><span class="sxs-lookup"><span data-stu-id="3f8ef-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f8ef-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f8ef-138">Response</span></span>

<span data-ttu-id="3f8ef-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-139">The following is an example of the response.</span></span>

> <span data-ttu-id="3f8ef-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="3f8ef-142">Запросы на /branding всегда возвращают **свойства mediaContentType,** **mediaReadLink** и **mediaEditLink.**</span><span class="sxs-lookup"><span data-stu-id="3f8ef-142">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="3f8ef-143">Если был применен локализ, **mediaEditLink** — это **mediaEditLink** для локального (который всегда не является null), а **mediaReadLink** и **mediaContentType** — **это mediaReadLink** и **mediaContentType** локального сайта, если **mediaReadLink** локального сайта не является null; в противном случае **по умолчанию mediaReadLink** и **mediaContentType**.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-143">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="3f8ef-144">Пример 2. Получить организационный брендинг, но не настроить брендинг</span><span class="sxs-lookup"><span data-stu-id="3f8ef-144">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="3f8ef-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f8ef-145">Request</span></span>

<span data-ttu-id="3f8ef-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="3f8ef-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f8ef-147">Response</span></span>

<span data-ttu-id="3f8ef-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="3f8ef-149">Пример 3. Получить организационный брендинг для французского языка</span><span class="sxs-lookup"><span data-stu-id="3f8ef-149">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="3f8ef-150">**Заготвка Accept-Language** используется для применения определенной локализации к брендингу.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-150">The **Accept-Language** header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="3f8ef-151">Свойства, `null` указанные в указанной локализации, возвращаются из фирменого бренда по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-151">Properties that are `null` in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="3f8ef-152">Если в **запросе указан** заглавный загон Accept-Language, ответ будет включать заглавный загон **Content-Language,** если это не `und` так.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-152">If the **Accept-Language** header is specified in the request, the response will include the **Content-Language** header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="3f8ef-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f8ef-153">Request</span></span>

<span data-ttu-id="3f8ef-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="3f8ef-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f8ef-155">Response</span></span>

<span data-ttu-id="3f8ef-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-156">The following is an example of the response.</span></span>

> <span data-ttu-id="3f8ef-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="3f8ef-159">Пример 4. Получить bannerLogo для французского языка</span><span class="sxs-lookup"><span data-stu-id="3f8ef-159">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="3f8ef-160">Возвращает **bannerLogo** для `fr` локального, если он существует.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-160">Returns **bannerLogo** for the `fr` locale if it exists.</span></span> <span data-ttu-id="3f8ef-161">Если локализация не существует, возвращается **баннер по умолчаниюLogo**.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-161">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="3f8ef-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f8ef-162">Request</span></span>

<span data-ttu-id="3f8ef-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f8ef-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f8ef-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_5"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```
# <a name="c"></a>[<span data-ttu-id="3f8ef-165">C#</span><span class="sxs-lookup"><span data-stu-id="3f8ef-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f8ef-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f8ef-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f8ef-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f8ef-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f8ef-168">Java</span><span class="sxs-lookup"><span data-stu-id="3f8ef-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f8ef-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f8ef-169">Response</span></span>

<span data-ttu-id="3f8ef-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-170">The following is an example of the response.</span></span>

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

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="3f8ef-171">Пример 5. Получить bannerLogo, когда не настроен bannerLogo</span><span class="sxs-lookup"><span data-stu-id="3f8ef-171">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="3f8ef-172">В этом примере показан запрос на свойство, которое не существует в фирменой марке по умолчанию или на языке, указанном в загородной головке **Accept-Language.**</span><span class="sxs-lookup"><span data-stu-id="3f8ef-172">This example shows a request for a property that does not exist on the default branding or the language specified in the **Accept-Language** header.</span></span>

#### <a name="request"></a><span data-ttu-id="3f8ef-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f8ef-173">Request</span></span>

<span data-ttu-id="3f8ef-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-174">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3f8ef-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f8ef-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_6"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```
# <a name="c"></a>[<span data-ttu-id="3f8ef-176">C#</span><span class="sxs-lookup"><span data-stu-id="3f8ef-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f8ef-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f8ef-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f8ef-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f8ef-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f8ef-179">Java</span><span class="sxs-lookup"><span data-stu-id="3f8ef-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f8ef-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f8ef-180">Response</span></span>

<span data-ttu-id="3f8ef-181">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3f8ef-181">The following is an example of the response.</span></span>

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
