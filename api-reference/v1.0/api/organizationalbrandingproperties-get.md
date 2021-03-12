---
title: Get organizationalBrandingProperties
description: Извлечение свойств и связей объекта organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: df77f6b26cab6324574ce22335e0b0c3236ee7b9
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722647"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="b7ef8-103">Get organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="b7ef8-103">Get organizationalBrandingProperties</span></span>

<span data-ttu-id="b7ef8-104">Извлечение свойств и связей объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="b7ef8-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7ef8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7ef8-105">Permissions</span></span>

<span data-ttu-id="b7ef8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7ef8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7ef8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7ef8-108">Permission type</span></span>                        | <span data-ttu-id="b7ef8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7ef8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b7ef8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7ef8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7ef8-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="b7ef8-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="b7ef8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7ef8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7ef8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-113">Not supported.</span></span> |
| <span data-ttu-id="b7ef8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7ef8-114">Application</span></span>                            | <span data-ttu-id="b7ef8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7ef8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7ef8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="b7ef8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7ef8-117">Request headers</span></span>

| <span data-ttu-id="b7ef8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b7ef8-118">Name</span></span>      |<span data-ttu-id="b7ef8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b7ef8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b7ef8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7ef8-120">Authorization</span></span> | <span data-ttu-id="b7ef8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-p102">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="b7ef8-123">При попытке запроса в Graph Explorer необходимо также включить заглавную головку запроса **Accept-Language** с допустимым локализом ISO-639.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-123">If you try the query in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="b7ef8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7ef8-124">Request body</span></span>

<span data-ttu-id="b7ef8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7ef8-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ef8-126">Response</span></span>

<span data-ttu-id="b7ef8-127">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-127">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7ef8-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b7ef8-128">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="b7ef8-129">Пример 1. Получить брендинг по умолчанию</span><span class="sxs-lookup"><span data-stu-id="b7ef8-129">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="b7ef8-130">Если вы попробуете пример в Graph Explorer, необходимо также включить заглавную головку запроса **Accept-Language** с допустимым локальным кодом ISO-639, чтобы избежать ошибки " Значение недействительный код локального языка *en-US,en;q=0.9. Это должен быть допустимый локал ISO-639.*</span><span class="sxs-lookup"><span data-stu-id="b7ef8-130">If you try the example in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale to avoid getting an error "*Invalid locale id value en-US,en;q=0.9. It must be a valid ISO-639 locale.*"</span></span>

#### <a name="request"></a><span data-ttu-id="b7ef8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7ef8-131">Request</span></span>

<span data-ttu-id="b7ef8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="b7ef8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ef8-133">Response</span></span>

<span data-ttu-id="b7ef8-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-134">The following is an example of the response.</span></span>

> <span data-ttu-id="b7ef8-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="b7ef8-137">Запросы на /branding всегда возвращают **свойства mediaContentType,** **mediaReadLink** и **mediaEditLink.**</span><span class="sxs-lookup"><span data-stu-id="b7ef8-137">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="b7ef8-138">Если был применен локализ, **mediaEditLink** — это **mediaEditLink** для локального (который всегда не является null), а **mediaReadLink** и **mediaContentType** — **это mediaReadLink** и **mediaContentType** локального сайта, если **mediaReadLink** локального сайта не является null; в противном случае **по умолчанию mediaReadLink** и **mediaContentType**.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-138">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="b7ef8-139">Пример 2. Получить организационный брендинг, но не настроить брендинг</span><span class="sxs-lookup"><span data-stu-id="b7ef8-139">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="b7ef8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7ef8-140">Request</span></span>

<span data-ttu-id="b7ef8-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="b7ef8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ef8-142">Response</span></span>

<span data-ttu-id="b7ef8-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="b7ef8-144">Пример 3. Получить организационный брендинг для французского языка</span><span class="sxs-lookup"><span data-stu-id="b7ef8-144">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="b7ef8-145">**Заготвка Accept-Language** используется для применения определенной локализации к брендингу.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-145">The **Accept-Language** header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="b7ef8-146">Свойства, `null` указанные в указанной локализации, возвращаются из фирменого бренда по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-146">Properties that are `null` in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="b7ef8-147">Если в **запросе указан** заглавный загон Accept-Language, ответ будет включать заглавный загон **Content-Language,** если это не `und` так.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-147">If the **Accept-Language** header is specified in the request, the response will include the **Content-Language** header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="b7ef8-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7ef8-148">Request</span></span>

<span data-ttu-id="b7ef8-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="b7ef8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ef8-150">Response</span></span>

<span data-ttu-id="b7ef8-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-151">The following is an example of the response.</span></span>

> <span data-ttu-id="b7ef8-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="b7ef8-154">Пример 4. Получить bannerLogo для французского языка</span><span class="sxs-lookup"><span data-stu-id="b7ef8-154">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="b7ef8-155">Возвращает **bannerLogo** для `fr` локального, если он существует.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-155">Returns **bannerLogo** for the `fr` locale if it exists.</span></span> <span data-ttu-id="b7ef8-156">Если локализация не существует, возвращается **баннер по умолчаниюLogo**.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-156">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="b7ef8-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7ef8-157">Request</span></span>

<span data-ttu-id="b7ef8-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="b7ef8-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ef8-159">Response</span></span>

<span data-ttu-id="b7ef8-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-160">The following is an example of the response.</span></span>

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

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="b7ef8-161">Пример 5. Получить bannerLogo, когда не настроен bannerLogo</span><span class="sxs-lookup"><span data-stu-id="b7ef8-161">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="b7ef8-162">В этом примере показан запрос на свойство, которое не существует в фирменой марке по умолчанию или на языке, указанном в загородной головке **Accept-Language.**</span><span class="sxs-lookup"><span data-stu-id="b7ef8-162">This example shows a request for a property that does not exist on the default branding or the language specified in the **Accept-Language** header.</span></span>

#### <a name="request"></a><span data-ttu-id="b7ef8-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7ef8-163">Request</span></span>

<span data-ttu-id="b7ef8-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-164">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```

#### <a name="response"></a><span data-ttu-id="b7ef8-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7ef8-165">Response</span></span>

<span data-ttu-id="b7ef8-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7ef8-166">The following is an example of the response.</span></span>

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
