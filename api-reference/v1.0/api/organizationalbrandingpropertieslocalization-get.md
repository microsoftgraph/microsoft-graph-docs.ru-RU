---
title: Получить локализованные организационные свойстваBranding
description: Извлечение объекта organizationalbrandingproperties для определенного локального объекта.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fd1650c1b4a0aff6b88caad9f63023d3652b605e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949275"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="39dc2-103">Get Localized organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="39dc2-103">Get Localized organizationalBrandingProperties</span></span>

<span data-ttu-id="39dc2-104">Извлечение свойств объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="39dc2-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39dc2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39dc2-105">Permissions</span></span>

<span data-ttu-id="39dc2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39dc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39dc2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39dc2-108">Permission type</span></span>                        | <span data-ttu-id="39dc2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39dc2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39dc2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39dc2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="39dc2-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="39dc2-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="39dc2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39dc2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39dc2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39dc2-113">Not supported.</span></span> |
| <span data-ttu-id="39dc2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39dc2-114">Application</span></span>                            | <span data-ttu-id="39dc2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39dc2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39dc2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39dc2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="39dc2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39dc2-117">Request headers</span></span>

| <span data-ttu-id="39dc2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="39dc2-118">Name</span></span>      |<span data-ttu-id="39dc2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="39dc2-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39dc2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39dc2-120">Authorization</span></span> | <span data-ttu-id="39dc2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39dc2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39dc2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39dc2-123">Content-Type</span></span>  | <span data-ttu-id="39dc2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39dc2-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39dc2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39dc2-126">Request body</span></span>

<span data-ttu-id="39dc2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39dc2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39dc2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dc2-128">Response</span></span>

<span data-ttu-id="39dc2-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="39dc2-129">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="39dc2-130">Значение "id" соответствует запрашиваемой локализации.</span><span class="sxs-lookup"><span data-stu-id="39dc2-130">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="39dc2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="39dc2-131">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="39dc2-132">Пример 1. Получить локализованный брендинг для определенного локального (fr)</span><span class="sxs-lookup"><span data-stu-id="39dc2-132">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="39dc2-133">Запрос GET для определенной локализации возвращает только значения для этой локализации.</span><span class="sxs-lookup"><span data-stu-id="39dc2-133">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="39dc2-134">Значения Null не будут заменены значениями из брендинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="39dc2-134">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="39dc2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="39dc2-135">Request</span></span>

<span data-ttu-id="39dc2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39dc2-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="39dc2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="39dc2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_8"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="39dc2-138">C#</span><span class="sxs-lookup"><span data-stu-id="39dc2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-8-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39dc2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39dc2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-8-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39dc2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39dc2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-8-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39dc2-141">Java</span><span class="sxs-lookup"><span data-stu-id="39dc2-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-8-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39dc2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dc2-142">Response</span></span>

<span data-ttu-id="39dc2-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39dc2-143">The following is an example of the response.</span></span>

> <span data-ttu-id="39dc2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39dc2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
"backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
"bannerLogo@odata.mediaContentType":"image/*",
"bannerLogo@odata.mediaReadLink": null,
"bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
"id":"fr",
"squareLogo@odata.mediaContentType":"image/*",
"squareLogo@odata.mediaReadLink": null,
"squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
"signInPageText":null,
"usernameHintText":null
}
```

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="39dc2-146">Пример 2. Получить все языковые локализации, которые были настроены</span><span class="sxs-lookup"><span data-stu-id="39dc2-146">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="39dc2-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="39dc2-147">Request</span></span>

<span data-ttu-id="39dc2-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39dc2-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="39dc2-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="39dc2-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_9"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```
# <a name="c"></a>[<span data-ttu-id="39dc2-150">C#</span><span class="sxs-lookup"><span data-stu-id="39dc2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-9-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39dc2-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39dc2-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-9-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39dc2-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39dc2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-9-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39dc2-153">Java</span><span class="sxs-lookup"><span data-stu-id="39dc2-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-9-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39dc2-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dc2-154">Response</span></span>

<span data-ttu-id="39dc2-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39dc2-155">The following is an example of the response.</span></span>

> <span data-ttu-id="39dc2-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39dc2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "backgroundImage@odata.mediaEditLink":"https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id":"en-us",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
   },
   {
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id":"fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":null,
    "usernameHintText":null
   }
 ]
}
```

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="39dc2-158">Пример 3. Получить значение signInPageText для определенного локального значения</span><span class="sxs-lookup"><span data-stu-id="39dc2-158">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="39dc2-159">Запрос свойства локализации возвращает это значение или 204, если значение null.</span><span class="sxs-lookup"><span data-stu-id="39dc2-159">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="39dc2-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="39dc2-160">Request</span></span>

<span data-ttu-id="39dc2-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39dc2-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="39dc2-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="39dc2-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_10"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```
# <a name="c"></a>[<span data-ttu-id="39dc2-163">C#</span><span class="sxs-lookup"><span data-stu-id="39dc2-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-10-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39dc2-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39dc2-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-10-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39dc2-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39dc2-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-10-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39dc2-166">Java</span><span class="sxs-lookup"><span data-stu-id="39dc2-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-10-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="39dc2-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="39dc2-167">Response</span></span>

<span data-ttu-id="39dc2-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="39dc2-168">The following is an example of the response.</span></span>

> <span data-ttu-id="39dc2-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39dc2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
