---
title: Получение локализованных Организатионалбрандингпропертиес
description: Получение объекта организатионалбрандингпропертиес для определенного языкового стандарта.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75ba4f8ef3202f95d7538ef6017d01e005db60c9
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031968"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="7b86d-103">Получение локализованных Организатионалбрандингпропертиес</span><span class="sxs-lookup"><span data-stu-id="7b86d-103">Get Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b86d-104">Получение свойств объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="7b86d-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b86d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b86d-105">Permissions</span></span>

<span data-ttu-id="7b86d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b86d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b86d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b86d-108">Permission type</span></span>                        | <span data-ttu-id="7b86d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b86d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7b86d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b86d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b86d-111">Organization. Read. ALL, User. Read, User. Read. ALL, User. ReadBasic. ALL</span><span class="sxs-lookup"><span data-stu-id="7b86d-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="7b86d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b86d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b86d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b86d-113">Not supported.</span></span> |
| <span data-ttu-id="7b86d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b86d-114">Application</span></span>                            | <span data-ttu-id="7b86d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b86d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b86d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b86d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b86d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7b86d-117">Optional query parameters</span></span>

<span data-ttu-id="7b86d-118">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7b86d-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7b86d-119">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7b86d-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b86d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b86d-120">Request headers</span></span>

| <span data-ttu-id="7b86d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7b86d-121">Name</span></span>      |<span data-ttu-id="7b86d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7b86d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b86d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b86d-123">Authorization</span></span> | <span data-ttu-id="7b86d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b86d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b86d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b86d-126">Content-Type</span></span>  | <span data-ttu-id="7b86d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b86d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b86d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b86d-129">Request body</span></span>

<span data-ttu-id="7b86d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7b86d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b86d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b86d-131">Response</span></span>

<span data-ttu-id="7b86d-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b86d-132">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="7b86d-133">Значение ID соответствует запрошенной локализации.</span><span class="sxs-lookup"><span data-stu-id="7b86d-133">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="7b86d-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="7b86d-134">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="7b86d-135">Пример 1: получение локализованного фирменного стиля для определенного языкового стандарта (fr)</span><span class="sxs-lookup"><span data-stu-id="7b86d-135">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="7b86d-136">Запрос GET на определенную локализацию возвращает только значения для этой локализации.</span><span class="sxs-lookup"><span data-stu-id="7b86d-136">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="7b86d-137">Значения NULL не будут заменены на имена, указанные в фирменной символике по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7b86d-137">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="7b86d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b86d-138">Request</span></span>

<span data-ttu-id="7b86d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b86d-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```

#### <a name="response"></a><span data-ttu-id="7b86d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b86d-140">Response</span></span>

<span data-ttu-id="7b86d-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b86d-141">The following is an example of the response.</span></span>

> <span data-ttu-id="7b86d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b86d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="7b86d-144">Пример 2: получение всех настроенных локализаций для определенных языков</span><span class="sxs-lookup"><span data-stu-id="7b86d-144">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="7b86d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b86d-145">Request</span></span>

<span data-ttu-id="7b86d-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b86d-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```

#### <a name="response"></a><span data-ttu-id="7b86d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b86d-147">Response</span></span>

<span data-ttu-id="7b86d-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b86d-148">The following is an example of the response.</span></span>

> <span data-ttu-id="7b86d-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b86d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="7b86d-151">Пример 3: получение значения Сигнинпажетекст для определенного языкового стандарта</span><span class="sxs-lookup"><span data-stu-id="7b86d-151">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="7b86d-152">При запросе свойства локализации возвращается это значение или 204, если значение равно null.</span><span class="sxs-lookup"><span data-stu-id="7b86d-152">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="7b86d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b86d-153">Request</span></span>

<span data-ttu-id="7b86d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b86d-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```

#### <a name="response"></a><span data-ttu-id="7b86d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b86d-155">Response</span></span>

<span data-ttu-id="7b86d-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7b86d-156">The following is an example of the response.</span></span>

> <span data-ttu-id="7b86d-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b86d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
