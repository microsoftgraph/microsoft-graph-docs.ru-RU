---
title: Получить локализованные организационные свойстваBranding
description: Извлечение объекта organizationalbrandingproperties для определенного локального объекта.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 24ba0c96df393accfefa5930a60b9ca186819ac2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722635"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="97d55-103">Get Localized organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="97d55-103">Get Localized organizationalBrandingProperties</span></span>

<span data-ttu-id="97d55-104">Извлечение свойств объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="97d55-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97d55-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97d55-105">Permissions</span></span>

<span data-ttu-id="97d55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97d55-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97d55-108">Permission type</span></span>                        | <span data-ttu-id="97d55-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97d55-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="97d55-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97d55-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="97d55-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="97d55-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="97d55-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97d55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97d55-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97d55-113">Not supported.</span></span> |
| <span data-ttu-id="97d55-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97d55-114">Application</span></span>                            | <span data-ttu-id="97d55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97d55-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97d55-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97d55-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="97d55-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97d55-117">Request headers</span></span>

| <span data-ttu-id="97d55-118">Имя</span><span class="sxs-lookup"><span data-stu-id="97d55-118">Name</span></span>      |<span data-ttu-id="97d55-119">Описание</span><span class="sxs-lookup"><span data-stu-id="97d55-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="97d55-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97d55-120">Authorization</span></span> | <span data-ttu-id="97d55-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97d55-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97d55-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97d55-123">Content-Type</span></span>  | <span data-ttu-id="97d55-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97d55-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97d55-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97d55-126">Request body</span></span>

<span data-ttu-id="97d55-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97d55-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97d55-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="97d55-128">Response</span></span>

<span data-ttu-id="97d55-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="97d55-129">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="97d55-130">Значение "id" соответствует запрашиваемой локализации.</span><span class="sxs-lookup"><span data-stu-id="97d55-130">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="97d55-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="97d55-131">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="97d55-132">Пример 1. Получить локализованный брендинг для определенного локального (fr)</span><span class="sxs-lookup"><span data-stu-id="97d55-132">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="97d55-133">Запрос GET для определенной локализации возвращает только значения для этой локализации.</span><span class="sxs-lookup"><span data-stu-id="97d55-133">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="97d55-134">Значения Null не будут заменены значениями из брендинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="97d55-134">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="97d55-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="97d55-135">Request</span></span>

<span data-ttu-id="97d55-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97d55-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```

#### <a name="response"></a><span data-ttu-id="97d55-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="97d55-137">Response</span></span>

<span data-ttu-id="97d55-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97d55-138">The following is an example of the response.</span></span>

> <span data-ttu-id="97d55-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97d55-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="97d55-141">Пример 2. Получить все языковые локализации, которые были настроены</span><span class="sxs-lookup"><span data-stu-id="97d55-141">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="97d55-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="97d55-142">Request</span></span>

<span data-ttu-id="97d55-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97d55-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```

#### <a name="response"></a><span data-ttu-id="97d55-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="97d55-144">Response</span></span>

<span data-ttu-id="97d55-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97d55-145">The following is an example of the response.</span></span>

> <span data-ttu-id="97d55-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97d55-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="97d55-148">Пример 3. Получить значение signInPageText для определенного локального значения</span><span class="sxs-lookup"><span data-stu-id="97d55-148">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="97d55-149">Запрос свойства локализации возвращает это значение или 204, если значение null.</span><span class="sxs-lookup"><span data-stu-id="97d55-149">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="97d55-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="97d55-150">Request</span></span>

<span data-ttu-id="97d55-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97d55-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```

#### <a name="response"></a><span data-ttu-id="97d55-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="97d55-152">Response</span></span>

<span data-ttu-id="97d55-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97d55-153">The following is an example of the response.</span></span>

> <span data-ttu-id="97d55-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97d55-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
