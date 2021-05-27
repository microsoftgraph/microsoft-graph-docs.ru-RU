---
title: Создание локализованных организационных свойствBrandingProperties
description: Создание фирменого бренда организации для определенного локального.
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 84e2ba2ed92533d552ba861f0d92dbde9cbf42ff
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680824"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="c8e2f-103">Создание локализованных организационных свойствBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="c8e2f-103">Create localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8e2f-104">Создание объекта [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) для определенного локального объекта.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8e2f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e2f-105">Permissions</span></span>

<span data-ttu-id="c8e2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8e2f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e2f-108">Permission type</span></span>                        | <span data-ttu-id="c8e2f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8e2f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8e2f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8e2f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8e2f-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e2f-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="c8e2f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8e2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8e2f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-113">Not supported.</span></span> |
| <span data-ttu-id="c8e2f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8e2f-114">Application</span></span>                            | <span data-ttu-id="c8e2f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8e2f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8e2f-116">HTTP request</span></span>

<span data-ttu-id="c8e2f-117">POST для создания новой локализации.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="c8e2f-118">Указанный в теле id — это локализовка для локализации.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="c8e2f-119">Если не указан id, то в качестве id используется значение загона Content-Language, если указано. Если не указаны id и не указаны заглавные материалы на языке контента, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{tenant id}/branding/localizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8e2f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8e2f-120">Optional query parameters</span></span>

<span data-ttu-id="c8e2f-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c8e2f-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c8e2f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8e2f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8e2f-123">Request headers</span></span>

| <span data-ttu-id="c8e2f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c8e2f-124">Name</span></span>      |<span data-ttu-id="c8e2f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e2f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8e2f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8e2f-126">Authorization</span></span> | <span data-ttu-id="c8e2f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8e2f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8e2f-129">Content-Type</span></span>  | <span data-ttu-id="c8e2f-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-p105">application/json. Required.</span></span>  |
| <span data-ttu-id="c8e2f-132">Content-Language</span><span class="sxs-lookup"><span data-stu-id="c8e2f-132">Content-Language</span></span>  | <span data-ttu-id="c8e2f-133">Locale.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-133">Locale.</span></span> <span data-ttu-id="c8e2f-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-134">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8e2f-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8e2f-135">Request body</span></span>

<span data-ttu-id="c8e2f-136">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-136">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c8e2f-137">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-137">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c8e2f-138">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-138">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c8e2f-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8e2f-139">Property</span></span>     | <span data-ttu-id="c8e2f-140">Тип</span><span class="sxs-lookup"><span data-stu-id="c8e2f-140">Type</span></span>        | <span data-ttu-id="c8e2f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e2f-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c8e2f-142">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="c8e2f-142">backgroundColor</span></span>|<span data-ttu-id="c8e2f-143">String</span><span class="sxs-lookup"><span data-stu-id="c8e2f-143">String</span></span>|<span data-ttu-id="c8e2f-144">Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-144">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="c8e2f-145">Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-145">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="c8e2f-146">Укажите это в hexadecimal (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="c8e2f-146">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="c8e2f-147">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="c8e2f-147">backgroundImage</span></span>|<span data-ttu-id="c8e2f-148">Stream</span><span class="sxs-lookup"><span data-stu-id="c8e2f-148">Stream</span></span>|<span data-ttu-id="c8e2f-149">Изображение, которое отображается в качестве фона знака на странице.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-149">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="c8e2f-150">.png или .jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-150">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="c8e2f-151">Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-151">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="c8e2f-152">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="c8e2f-152">bannerLogo</span></span>|<span data-ttu-id="c8e2f-153">Stream</span><span class="sxs-lookup"><span data-stu-id="c8e2f-153">Stream</span></span>|<span data-ttu-id="c8e2f-154">На странице входного знака отображается баннерная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-154">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="c8e2f-155">.png или .jpg не превышает 36x245px.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-155">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="c8e2f-156">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-156">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="c8e2f-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="c8e2f-157">signInPageText</span></span>|<span data-ttu-id="c8e2f-158">String</span><span class="sxs-lookup"><span data-stu-id="c8e2f-158">String</span></span>|<span data-ttu-id="c8e2f-159">Текст, который отображается в нижней части окна для регистрации.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="c8e2f-160">С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="c8e2f-161">Этот текст должен быть unicode и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-161">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="c8e2f-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="c8e2f-162">squareLogo</span></span>|<span data-ttu-id="c8e2f-163">Stream</span><span class="sxs-lookup"><span data-stu-id="c8e2f-163">Stream</span></span>|<span data-ttu-id="c8e2f-164">Квадратная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-164">Square version of your company logo.</span></span> <span data-ttu-id="c8e2f-165">Это отображается в Windows 10(OOBE) и когда Windows автопилот включен для развертывания.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="c8e2f-166">.png или .jpg размером не более 240x240px и не более 10 кб.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="c8e2f-167">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-167">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="c8e2f-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="c8e2f-168">usernameHintText</span></span>|<span data-ttu-id="c8e2f-169">String</span><span class="sxs-lookup"><span data-stu-id="c8e2f-169">String</span></span>|<span data-ttu-id="c8e2f-170">Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране знака.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="c8e2f-171">Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="c8e2f-172">id</span><span class="sxs-lookup"><span data-stu-id="c8e2f-172">id</span></span>|<span data-ttu-id="c8e2f-173">String</span><span class="sxs-lookup"><span data-stu-id="c8e2f-173">String</span></span>|<span data-ttu-id="c8e2f-174">Locale для создания брендинга для</span><span class="sxs-lookup"><span data-stu-id="c8e2f-174">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="c8e2f-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e2f-175">Response</span></span>

<span data-ttu-id="c8e2f-176">В случае успешной работы этот метод возвращает код ответа и созданный `201 CREATED` [объект organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-176">If successful, this method returns a `201 CREATED` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8e2f-177">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8e2f-177">Examples</span></span>

<span data-ttu-id="c8e2f-178">В следующем примере создается локализация бренда для французского языка (fr).</span><span class="sxs-lookup"><span data-stu-id="c8e2f-178">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="c8e2f-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8e2f-179">Request</span></span>

<span data-ttu-id="c8e2f-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8e2f-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8e2f-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_7"
}-->

```http
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="c8e2f-182">C#</span><span class="sxs-lookup"><span data-stu-id="c8e2f-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-7-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8e2f-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8e2f-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-7-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8e2f-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8e2f-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-7-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8e2f-185">Java</span><span class="sxs-lookup"><span data-stu-id="c8e2f-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-7-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8e2f-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e2f-186">Response</span></span>

<span data-ttu-id="c8e2f-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-187">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
<span data-ttu-id="c8e2f-188">**MediaEditLink** указывает, где записано локализованные носители.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-188">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="c8e2f-189">MediaReadLink является null, так как для локализации не установлено мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c8e2f-189">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
