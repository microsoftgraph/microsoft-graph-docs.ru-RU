---
title: Создание локализованных организационных свойствBrandingProperties
description: Создание фирменого бренда организации для определенного локального.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 03ecb7805a47216bb4d4643c9a0b3036139069ad
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949299"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="76fed-103">Создание локализованных организационных свойствBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="76fed-103">Create localized organizationalBrandingProperties</span></span>

<span data-ttu-id="76fed-104">Создание объекта [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) для определенного локального объекта.</span><span class="sxs-lookup"><span data-stu-id="76fed-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="76fed-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76fed-105">Permissions</span></span>

<span data-ttu-id="76fed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76fed-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76fed-108">Permission type</span></span>                        | <span data-ttu-id="76fed-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76fed-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76fed-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76fed-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="76fed-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76fed-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="76fed-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76fed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76fed-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76fed-113">Not supported.</span></span> |
| <span data-ttu-id="76fed-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76fed-114">Application</span></span>                            | <span data-ttu-id="76fed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76fed-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76fed-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76fed-116">HTTP request</span></span>

<span data-ttu-id="76fed-117">POST для создания новой локализации.</span><span class="sxs-lookup"><span data-stu-id="76fed-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="76fed-118">Указанный в теле id — это локализовка для локализации.</span><span class="sxs-lookup"><span data-stu-id="76fed-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="76fed-119">Если не указан id, то в качестве id используется значение загона Content-Language, если указано. Если не указаны id и не указаны заглавные материалы на языке контента, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="76fed-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="request-headers"></a><span data-ttu-id="76fed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76fed-120">Request headers</span></span>

| <span data-ttu-id="76fed-121">Имя</span><span class="sxs-lookup"><span data-stu-id="76fed-121">Name</span></span>      |<span data-ttu-id="76fed-122">Описание</span><span class="sxs-lookup"><span data-stu-id="76fed-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76fed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76fed-123">Authorization</span></span> | <span data-ttu-id="76fed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76fed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76fed-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76fed-126">Content-Type</span></span>  | <span data-ttu-id="76fed-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76fed-p104">application/json. Required.</span></span>  |
| <span data-ttu-id="76fed-129">Content-Language</span><span class="sxs-lookup"><span data-stu-id="76fed-129">Content-Language</span></span>  | <span data-ttu-id="76fed-130">Locale.</span><span class="sxs-lookup"><span data-stu-id="76fed-130">Locale.</span></span> <span data-ttu-id="76fed-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="76fed-131">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76fed-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76fed-132">Request body</span></span>

<span data-ttu-id="76fed-133">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="76fed-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="76fed-134">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="76fed-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="76fed-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="76fed-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="76fed-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="76fed-136">Property</span></span>     | <span data-ttu-id="76fed-137">Тип</span><span class="sxs-lookup"><span data-stu-id="76fed-137">Type</span></span>        | <span data-ttu-id="76fed-138">Описание</span><span class="sxs-lookup"><span data-stu-id="76fed-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="76fed-139">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="76fed-139">backgroundColor</span></span>|<span data-ttu-id="76fed-140">Строка</span><span class="sxs-lookup"><span data-stu-id="76fed-140">String</span></span>|<span data-ttu-id="76fed-141">Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="76fed-141">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="76fed-142">Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации.</span><span class="sxs-lookup"><span data-stu-id="76fed-142">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="76fed-143">Укажите это в hexadecimal (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="76fed-143">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="76fed-144">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="76fed-144">backgroundImage</span></span>|<span data-ttu-id="76fed-145">Stream</span><span class="sxs-lookup"><span data-stu-id="76fed-145">Stream</span></span>|<span data-ttu-id="76fed-146">Изображение, которое отображается в качестве фона знака на странице.</span><span class="sxs-lookup"><span data-stu-id="76fed-146">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="76fed-147">.png или .jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="76fed-147">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="76fed-148">Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.</span><span class="sxs-lookup"><span data-stu-id="76fed-148">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="76fed-149">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="76fed-149">bannerLogo</span></span>|<span data-ttu-id="76fed-150">Stream</span><span class="sxs-lookup"><span data-stu-id="76fed-150">Stream</span></span>|<span data-ttu-id="76fed-151">На странице входного знака отображается баннерная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="76fed-151">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="76fed-152">.png или .jpg не больше 36x245px.</span><span class="sxs-lookup"><span data-stu-id="76fed-152">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="76fed-153">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="76fed-153">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="76fed-154">signInPageText</span><span class="sxs-lookup"><span data-stu-id="76fed-154">signInPageText</span></span>|<span data-ttu-id="76fed-155">Строка</span><span class="sxs-lookup"><span data-stu-id="76fed-155">String</span></span>|<span data-ttu-id="76fed-156">Текст, который отображается в нижней части окна для регистрации.</span><span class="sxs-lookup"><span data-stu-id="76fed-156">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="76fed-157">С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="76fed-157">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="76fed-158">Этот текст должен быть unicode и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="76fed-158">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="76fed-159">squareLogo</span><span class="sxs-lookup"><span data-stu-id="76fed-159">squareLogo</span></span>|<span data-ttu-id="76fed-160">Stream</span><span class="sxs-lookup"><span data-stu-id="76fed-160">Stream</span></span>|<span data-ttu-id="76fed-161">Квадратная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="76fed-161">Square version of your company logo.</span></span> <span data-ttu-id="76fed-162">Это отображается в windows 10 вне окна (OOBE) опытом и когда Windows Автопилот включен для развертывания.</span><span class="sxs-lookup"><span data-stu-id="76fed-162">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="76fed-163">.png или .jpg размером не более 240x240px и размером не более 10 кб.</span><span class="sxs-lookup"><span data-stu-id="76fed-163">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="76fed-164">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="76fed-164">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="76fed-165">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="76fed-165">usernameHintText</span></span>|<span data-ttu-id="76fed-166">Строка</span><span class="sxs-lookup"><span data-stu-id="76fed-166">String</span></span>|<span data-ttu-id="76fed-167">Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране знака.</span><span class="sxs-lookup"><span data-stu-id="76fed-167">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="76fed-168">Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="76fed-168">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="76fed-169">id</span><span class="sxs-lookup"><span data-stu-id="76fed-169">id</span></span>|<span data-ttu-id="76fed-170">Строка</span><span class="sxs-lookup"><span data-stu-id="76fed-170">String</span></span>|<span data-ttu-id="76fed-171">Locale для создания брендинга для</span><span class="sxs-lookup"><span data-stu-id="76fed-171">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="76fed-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="76fed-172">Response</span></span>

<span data-ttu-id="76fed-173">В случае успешной работы этот метод возвращает код ответа и созданный `201 Created` [объект organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="76fed-173">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76fed-174">Примеры</span><span class="sxs-lookup"><span data-stu-id="76fed-174">Examples</span></span>

<span data-ttu-id="76fed-175">В следующем примере создается локализация бренда для французского языка (fr).</span><span class="sxs-lookup"><span data-stu-id="76fed-175">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="76fed-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="76fed-176">Request</span></span>

<span data-ttu-id="76fed-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76fed-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="76fed-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="76fed-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_7"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="76fed-179">C#</span><span class="sxs-lookup"><span data-stu-id="76fed-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-7-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="76fed-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76fed-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-7-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76fed-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76fed-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-7-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="76fed-182">Java</span><span class="sxs-lookup"><span data-stu-id="76fed-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-7-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76fed-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="76fed-183">Response</span></span>

<span data-ttu-id="76fed-184">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="76fed-184">The following is an example of the response.</span></span>

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
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
<span data-ttu-id="76fed-185">**MediaEditLink** указывает, где записано локализованные носители.</span><span class="sxs-lookup"><span data-stu-id="76fed-185">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="76fed-186">MediaReadLink является null, так как для локализации не установлено мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="76fed-186">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
