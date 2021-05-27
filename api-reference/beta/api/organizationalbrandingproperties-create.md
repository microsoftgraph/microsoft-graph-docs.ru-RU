---
title: Создание organizationalBrandingProperties
description: Создание фирменого бренда организации.
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d74061ce6f323818ee77789db59def46048fa7f7
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679654"
---
# <a name="create-organizationalbrandingproperties"></a><span data-ttu-id="d327d-103">Создание organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="d327d-103">Create organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d327d-104">Создание [объекта organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="d327d-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="d327d-105">Это создает брендинг по умолчанию и одновременно локализованный брендинг.</span><span class="sxs-lookup"><span data-stu-id="d327d-105">This creates the default branding and optionally a localized branding at the same time.</span></span> <span data-ttu-id="d327d-106">Брендинг по умолчанию загружается, когда локализованный набор брендинга не настроен на язык браузера пользователя.</span><span class="sxs-lookup"><span data-stu-id="d327d-106">The default branding is loaded when a localized branding set isn't configured for the user's browser language.</span></span>

## <a name="permissions"></a><span data-ttu-id="d327d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d327d-107">Permissions</span></span>

<span data-ttu-id="d327d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d327d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d327d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d327d-110">Permission type</span></span>                        | <span data-ttu-id="d327d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d327d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d327d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d327d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d327d-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d327d-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="d327d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d327d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d327d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d327d-115">Not supported.</span></span> |
| <span data-ttu-id="d327d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d327d-116">Application</span></span>                            | <span data-ttu-id="d327d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d327d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d327d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d327d-118">HTTP request</span></span>

<span data-ttu-id="d327d-119">Брендинг создается для организации, если она еще не существует, с помощью PUT или PATCH.</span><span class="sxs-lookup"><span data-stu-id="d327d-119">A branding is created for an organization, if one does not already exist, using PUT or PATCH.</span></span>

<span data-ttu-id="d327d-120">Если брендинг уже настроен, PUT переопишет все существующие значения независимо от того, что находится в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="d327d-120">If branding is already configured, PUT will overwrite all existing values regardless of what's in the request body.</span></span> <span data-ttu-id="d327d-121">PATCH будет только заорит значения, включенные в тело запроса, в результате чего значения не будут включены без изменений.</span><span class="sxs-lookup"><span data-stu-id="d327d-121">PATCH will only overite the values that are included in the request body, leaving the values not included unchanged.</span></span>

<span data-ttu-id="d327d-122">Свойство **id** игнорируется в PUT/PATCH в синглтоне /branding.</span><span class="sxs-lookup"><span data-stu-id="d327d-122">The **id** property is ignored on PUT/PATCH to the /branding singleton.</span></span> <span data-ttu-id="d327d-123">Если язык контента не указан, создается брендинг по умолчанию, соответствующий **id** `und` .</span><span class="sxs-lookup"><span data-stu-id="d327d-123">If Content-Language is not specified, the default branding is created, which corresponds to an **id** of `und`.</span></span> <span data-ttu-id="d327d-124">Если задан язык контента, для этого языка создается брендинг.</span><span class="sxs-lookup"><span data-stu-id="d327d-124">If Content-Language is specified, branding is created for that locale.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{tenant id}/branding
PATCH /organization/{tenant id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d327d-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d327d-125">Optional query parameters</span></span>

<span data-ttu-id="d327d-126">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d327d-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d327d-127">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d327d-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d327d-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d327d-128">Request headers</span></span>

| <span data-ttu-id="d327d-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d327d-129">Name</span></span>      |<span data-ttu-id="d327d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d327d-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d327d-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d327d-131">Authorization</span></span> | <span data-ttu-id="d327d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d327d-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d327d-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d327d-134">Content-Type</span></span>  | <span data-ttu-id="d327d-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d327d-p107">application/json. Required.</span></span>  |
| <span data-ttu-id="d327d-137">Content-Language</span><span class="sxs-lookup"><span data-stu-id="d327d-137">Content-Language</span></span>  | <span data-ttu-id="d327d-138">Locale.</span><span class="sxs-lookup"><span data-stu-id="d327d-138">Locale.</span></span> <span data-ttu-id="d327d-139">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d327d-139">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d327d-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d327d-140">Request body</span></span>

| <span data-ttu-id="d327d-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="d327d-141">Property</span></span>     | <span data-ttu-id="d327d-142">Тип</span><span class="sxs-lookup"><span data-stu-id="d327d-142">Type</span></span>        | <span data-ttu-id="d327d-143">Описание</span><span class="sxs-lookup"><span data-stu-id="d327d-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d327d-144">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="d327d-144">backgroundColor</span></span>|<span data-ttu-id="d327d-145">String</span><span class="sxs-lookup"><span data-stu-id="d327d-145">String</span></span>|<span data-ttu-id="d327d-146">Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="d327d-146">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="d327d-147">Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации.</span><span class="sxs-lookup"><span data-stu-id="d327d-147">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="d327d-148">Укажите это в hexadecimal (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="d327d-148">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="d327d-149">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="d327d-149">backgroundImage</span></span>|<span data-ttu-id="d327d-150">Stream</span><span class="sxs-lookup"><span data-stu-id="d327d-150">Stream</span></span>|<span data-ttu-id="d327d-151">Изображение, которое отображается в качестве фона знака на странице.</span><span class="sxs-lookup"><span data-stu-id="d327d-151">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="d327d-152">.png или .jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="d327d-152">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="d327d-153">Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.</span><span class="sxs-lookup"><span data-stu-id="d327d-153">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="d327d-154">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="d327d-154">bannerLogo</span></span>|<span data-ttu-id="d327d-155">Stream</span><span class="sxs-lookup"><span data-stu-id="d327d-155">Stream</span></span>|<span data-ttu-id="d327d-156">На странице входного знака отображается баннерная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="d327d-156">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="d327d-157">.png или .jpg не превышает 36x245px.</span><span class="sxs-lookup"><span data-stu-id="d327d-157">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="d327d-158">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="d327d-158">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="d327d-159">signInPageText</span><span class="sxs-lookup"><span data-stu-id="d327d-159">signInPageText</span></span>|<span data-ttu-id="d327d-160">String</span><span class="sxs-lookup"><span data-stu-id="d327d-160">String</span></span>|<span data-ttu-id="d327d-161">Текст, который отображается в нижней части окна для регистрации.</span><span class="sxs-lookup"><span data-stu-id="d327d-161">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="d327d-162">С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="d327d-162">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="d327d-163">Этот текст должен быть unicode и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="d327d-163">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="d327d-164">squareLogo</span><span class="sxs-lookup"><span data-stu-id="d327d-164">squareLogo</span></span>|<span data-ttu-id="d327d-165">Stream</span><span class="sxs-lookup"><span data-stu-id="d327d-165">Stream</span></span>|<span data-ttu-id="d327d-166">Квадратная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="d327d-166">Square version of your company logo.</span></span> <span data-ttu-id="d327d-167">Это отображается в Windows 10(OOBE) и когда Windows автопилот включен для развертывания.</span><span class="sxs-lookup"><span data-stu-id="d327d-167">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="d327d-168">.png или .jpg размером не более 240x240px и не более 10 кб.</span><span class="sxs-lookup"><span data-stu-id="d327d-168">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="d327d-169">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="d327d-169">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="d327d-170">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="d327d-170">usernameHintText</span></span>|<span data-ttu-id="d327d-171">String</span><span class="sxs-lookup"><span data-stu-id="d327d-171">String</span></span>|<span data-ttu-id="d327d-172">Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране знака.</span><span class="sxs-lookup"><span data-stu-id="d327d-172">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="d327d-173">Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="d327d-173">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="d327d-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="d327d-174">Response</span></span>

<span data-ttu-id="d327d-175">В случае успешной работы этот метод возвращает код ответа и созданный `201 Created` [объект organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d327d-175">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d327d-176">Примеры</span><span class="sxs-lookup"><span data-stu-id="d327d-176">Examples</span></span>

<span data-ttu-id="d327d-177">В следующем примере создается брендинг по умолчанию и локализация для en-US.</span><span class="sxs-lookup"><span data-stu-id="d327d-177">The following example creates default branding and localization for en-US.</span></span>

### <a name="request"></a><span data-ttu-id="d327d-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="d327d-178">Request</span></span>

<span data-ttu-id="d327d-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d327d-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d327d-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="d327d-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_1"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```
# <a name="c"></a>[<span data-ttu-id="d327d-181">C#</span><span class="sxs-lookup"><span data-stu-id="d327d-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d327d-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d327d-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d327d-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d327d-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d327d-184">Java</span><span class="sxs-lookup"><span data-stu-id="d327d-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d327d-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="d327d-185">Response</span></span>

<span data-ttu-id="d327d-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d327d-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

<span data-ttu-id="d327d-187">В этом случае заданной является объект брендинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d327d-187">In this case, the default branding object is set.</span></span> <span data-ttu-id="d327d-188">Локализованный брендинг для en-US также устанавливается из-за языка контента в загонке, даже если набор брендинга en-US не возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="d327d-188">Localized branding for en-US is also set due to the Content-Language in the header, even though the en-US branding set is not returned in the response.</span></span> <span data-ttu-id="d327d-189">Обратите внимание, что язык контента в запросе необязателен, а если нет, будет устанавливаться только брендинг по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d327d-189">Note that Content-Language in the request is optional, and if not present, will only set default branding.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
