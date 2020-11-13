---
title: Получение Организатионалбрандингпропертиес
description: Получение свойств и связей объекта Организатионалбрандингпропертиес.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f46f6487fc067aaab780f06395f5ff2b5b682f80
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031980"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="33dd2-103">Получение Организатионалбрандингпропертиес</span><span class="sxs-lookup"><span data-stu-id="33dd2-103">Get organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33dd2-104">Получение свойств и связей объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="33dd2-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="33dd2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33dd2-105">Permissions</span></span>

<span data-ttu-id="33dd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33dd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33dd2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33dd2-108">Permission type</span></span>                        | <span data-ttu-id="33dd2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33dd2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="33dd2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33dd2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="33dd2-111">Organization. Read. ALL, User. Read, User. Read. ALL, User. ReadBasic. ALL</span><span class="sxs-lookup"><span data-stu-id="33dd2-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="33dd2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33dd2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33dd2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33dd2-113">Not supported.</span></span> |
| <span data-ttu-id="33dd2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33dd2-114">Application</span></span>                            | <span data-ttu-id="33dd2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33dd2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33dd2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33dd2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/{property name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33dd2-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="33dd2-117">Optional query parameters</span></span>

<span data-ttu-id="33dd2-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="33dd2-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="33dd2-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="33dd2-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="33dd2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33dd2-120">Request headers</span></span>

| <span data-ttu-id="33dd2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="33dd2-121">Name</span></span>      |<span data-ttu-id="33dd2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="33dd2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33dd2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33dd2-123">Authorization</span></span> | <span data-ttu-id="33dd2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33dd2-p103">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="33dd2-126">Если вы попробуете выполнить запрос в проводнике Graph, необходимо также добавить заголовок запроса Accept-Language с допустимым языковым стандартом ISO-639.</span><span class="sxs-lookup"><span data-stu-id="33dd2-126">If you try the query in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="33dd2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33dd2-127">Request body</span></span>

<span data-ttu-id="33dd2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33dd2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33dd2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="33dd2-129">Response</span></span>

<span data-ttu-id="33dd2-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33dd2-130">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33dd2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="33dd2-131">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="33dd2-132">Пример 1: получение фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="33dd2-132">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="33dd2-133">Если вы попробуете пример в проводнике Graph, необходимо также добавить заголовок запроса Accept-Language с допустимым языковым стандартом ISO-639, чтобы избежать ошибки "Недопустимый код языка — en-US, EN; q = 0.9.</span><span class="sxs-lookup"><span data-stu-id="33dd2-133">If you try the example in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale to avoid getting an error "Invalid locale id value en-US,en;q=0.9.</span></span> <span data-ttu-id="33dd2-134">Он должен быть допустимым языковым стандартом ISO-639. "</span><span class="sxs-lookup"><span data-stu-id="33dd2-134">It must be a valid ISO-639 locale."</span></span>

#### <a name="request"></a><span data-ttu-id="33dd2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="33dd2-135">Request</span></span>

<span data-ttu-id="33dd2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33dd2-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="33dd2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="33dd2-137">Response</span></span>

<span data-ttu-id="33dd2-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33dd2-138">The following is an example of the response.</span></span>

> <span data-ttu-id="33dd2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33dd2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="33dd2-141">Запросы для/брандинг всегда возвращают свойства **медиаконтенттипе** , **медиареадлинк** и **медиаедитлинк** .</span><span class="sxs-lookup"><span data-stu-id="33dd2-141">Requests for /branding always return the **mediaContentType** , **mediaReadLink** , and **mediaEditLink** properties.</span></span> <span data-ttu-id="33dd2-142">Если применен языковой стандарт, **медиаедитлинк** является **медиаедитлинк** для языкового стандарта (который всегда имеет значение, отличное от NULL), а **Медиареадлинк** и **медиаконтенттипе** — это **Медиареадлинк** и **медиаконтенттипе** для языкового стандарта, если **mediaReadLink** языкового стандарта не имеет значение null; в противном случае — **медиареадлинк** и **медиаконтенттипе** по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33dd2-142">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="33dd2-143">Пример 2: получение фирменной символики Организации, но не настроена фирменная символика</span><span class="sxs-lookup"><span data-stu-id="33dd2-143">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="33dd2-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="33dd2-144">Request</span></span>

<span data-ttu-id="33dd2-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33dd2-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="33dd2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="33dd2-146">Response</span></span>

<span data-ttu-id="33dd2-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33dd2-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="33dd2-148">Пример 3: получение фирменной символики для французского языка</span><span class="sxs-lookup"><span data-stu-id="33dd2-148">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="33dd2-149">Заголовок Accept-Langauge используется для применения определенной локализации к фирменной символике.</span><span class="sxs-lookup"><span data-stu-id="33dd2-149">The Accept-Langauge header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="33dd2-150">Свойства, которые имеют значение NULL в указанной локализации, возвращаются из фирменной символики по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33dd2-150">Properties that are null in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="33dd2-151">Если заголовок Accept-Language указан в запросе, в ответ будет включен заголовок Content-Language, если это не так `und` .</span><span class="sxs-lookup"><span data-stu-id="33dd2-151">If the Accept-Language header is specified in the request, the response will include the Content-Language header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="33dd2-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="33dd2-152">Request</span></span>

<span data-ttu-id="33dd2-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33dd2-153">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="33dd2-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="33dd2-154">Response</span></span>

<span data-ttu-id="33dd2-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33dd2-155">The following is an example of the response.</span></span>

> <span data-ttu-id="33dd2-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33dd2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="33dd2-158">Пример 4: Get Баннерлого для французского языка</span><span class="sxs-lookup"><span data-stu-id="33dd2-158">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="33dd2-159">Возвращает **баннерлого** для языкового стандарта fr, если он существует.</span><span class="sxs-lookup"><span data-stu-id="33dd2-159">Returns **bannerLogo** for the fr locale if it exists.</span></span> <span data-ttu-id="33dd2-160">Если локализация не существует, возвращается **баннерлого** по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="33dd2-160">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="33dd2-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="33dd2-161">Request</span></span>

<span data-ttu-id="33dd2-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33dd2-162">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="33dd2-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="33dd2-163">Response</span></span>

<span data-ttu-id="33dd2-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33dd2-164">The following is an example of the response.</span></span>

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

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="33dd2-165">Пример 5: Get Баннерлого, если не настроен ни один Баннерлого</span><span class="sxs-lookup"><span data-stu-id="33dd2-165">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="33dd2-166">В этом примере показан запрос для свойства, которое не существует на фирменной символике по умолчанию или на языке, указанном в заголовке Accept-Language.</span><span class="sxs-lookup"><span data-stu-id="33dd2-166">This example shows a request for a property that does not exist on the default branding or the language specified in the Accept-Language header.</span></span>

#### <a name="request"></a><span data-ttu-id="33dd2-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="33dd2-167">Request</span></span>

<span data-ttu-id="33dd2-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33dd2-168">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```

#### <a name="response"></a><span data-ttu-id="33dd2-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="33dd2-169">Response</span></span>

<span data-ttu-id="33dd2-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="33dd2-170">The following is an example of the response.</span></span>

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
