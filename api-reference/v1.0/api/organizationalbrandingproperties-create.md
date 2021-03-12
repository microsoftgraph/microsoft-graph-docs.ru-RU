---
title: Создание organizationalBrandingProperties
description: Создание фирменого бренда организации.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6f5e16a87f78be5e0664af624d058fff64f70bba
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722670"
---
# <a name="create-organizationalbrandingproperties"></a><span data-ttu-id="095fc-103">Создание organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="095fc-103">Create organizationalBrandingProperties</span></span>

<span data-ttu-id="095fc-104">Создание [объекта organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="095fc-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="095fc-105">Это создает брендинг по умолчанию и необязательно локализованный брендинг.</span><span class="sxs-lookup"><span data-stu-id="095fc-105">This creates the default branding and optionally a localized branding.</span></span> <span data-ttu-id="095fc-106">Брендинг по умолчанию загружается, когда локализованный набор брендинга не настроен на язык браузера пользователя.</span><span class="sxs-lookup"><span data-stu-id="095fc-106">The default branding is loaded when a localized branding set isn't configured for the user's browser language.</span></span>

## <a name="permissions"></a><span data-ttu-id="095fc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="095fc-107">Permissions</span></span>

<span data-ttu-id="095fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="095fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="095fc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="095fc-110">Permission type</span></span>                        | <span data-ttu-id="095fc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="095fc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="095fc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="095fc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="095fc-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="095fc-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="095fc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="095fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="095fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="095fc-115">Not supported.</span></span> |
| <span data-ttu-id="095fc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="095fc-116">Application</span></span>                            | <span data-ttu-id="095fc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="095fc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="095fc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="095fc-118">HTTP request</span></span>

<span data-ttu-id="095fc-119">Брендинг создается для организации, если она еще не существует, с помощью PUT или PATCH.</span><span class="sxs-lookup"><span data-stu-id="095fc-119">A branding is created for an organization, if one does not already exist, using PUT or PATCH.</span></span>

<span data-ttu-id="095fc-120">Если брендинг уже настроен, PUT переописает все существующие значения независимо от того, что находится в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="095fc-120">If branding is already configured, PUT overwrites all existing values regardless of what's in the request body.</span></span> <span data-ttu-id="095fc-121">PATCH только переописывает значения, включенные в тело запроса, в результате чего значения не остаются неизменными.</span><span class="sxs-lookup"><span data-stu-id="095fc-121">PATCH only overwrites the values that are included in the request body, leaving the values not included unchanged.</span></span>

<span data-ttu-id="095fc-122">Свойство `id` игнорируется в PUT/PATCH в синглтоне /branding.</span><span class="sxs-lookup"><span data-stu-id="095fc-122">The `id` property is ignored on PUT/PATCH to the /branding singleton.</span></span> <span data-ttu-id="095fc-123">Если **язык контента** не указан, создается брендинг по умолчанию, соответствующий `id` одному из `und` .</span><span class="sxs-lookup"><span data-stu-id="095fc-123">If **Content-Language** is not specified, the default branding is created, which corresponds to an `id` of `und`.</span></span> <span data-ttu-id="095fc-124">Если **задан язык** контента, для этого языка создается брендинг.</span><span class="sxs-lookup"><span data-stu-id="095fc-124">If **Content-Language** is specified, branding is created for that locale.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="095fc-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="095fc-125">Request headers</span></span>

| <span data-ttu-id="095fc-126">Имя</span><span class="sxs-lookup"><span data-stu-id="095fc-126">Name</span></span>      |<span data-ttu-id="095fc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="095fc-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="095fc-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="095fc-128">Authorization</span></span> | <span data-ttu-id="095fc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="095fc-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="095fc-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="095fc-131">Content-Type</span></span>  | <span data-ttu-id="095fc-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="095fc-p106">application/json. Required.</span></span>  |
| <span data-ttu-id="095fc-134">Content-Language</span><span class="sxs-lookup"><span data-stu-id="095fc-134">Content-Language</span></span>  | <span data-ttu-id="095fc-135">Locale.</span><span class="sxs-lookup"><span data-stu-id="095fc-135">Locale.</span></span> <span data-ttu-id="095fc-136">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="095fc-136">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="095fc-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="095fc-137">Request body</span></span>

<span data-ttu-id="095fc-138">В орган запроса включаем представление JSON объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="095fc-138">In the request body, include a JSON representation of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="095fc-139">В следующей таблице перечислены необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="095fc-139">The following table lists the required properties.</span></span>

| <span data-ttu-id="095fc-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="095fc-140">Property</span></span>     | <span data-ttu-id="095fc-141">Тип</span><span class="sxs-lookup"><span data-stu-id="095fc-141">Type</span></span>        | <span data-ttu-id="095fc-142">Описание</span><span class="sxs-lookup"><span data-stu-id="095fc-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="095fc-143">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="095fc-143">backgroundColor</span></span>|<span data-ttu-id="095fc-144">String</span><span class="sxs-lookup"><span data-stu-id="095fc-144">String</span></span>|<span data-ttu-id="095fc-145">Цвет, который отображается на месте фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="095fc-145">Color that appears in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="095fc-146">Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации.</span><span class="sxs-lookup"><span data-stu-id="095fc-146">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="095fc-147">Укажите это в hexadecimal (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="095fc-147">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="095fc-148">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="095fc-148">backgroundImage</span></span>|<span data-ttu-id="095fc-149">Stream</span><span class="sxs-lookup"><span data-stu-id="095fc-149">Stream</span></span>|<span data-ttu-id="095fc-150">Изображение, которое отображается в качестве фона страницы регистрации.</span><span class="sxs-lookup"><span data-stu-id="095fc-150">Image that appears as the background of the sign-in page.</span></span> <span data-ttu-id="095fc-151">Изображение — это .png или .jpg, размером не более 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="095fc-151">The image is a .png or .jpg that is not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="095fc-152">Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.</span><span class="sxs-lookup"><span data-stu-id="095fc-152">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="095fc-153">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="095fc-153">bannerLogo</span></span>|<span data-ttu-id="095fc-154">Stream</span><span class="sxs-lookup"><span data-stu-id="095fc-154">Stream</span></span>|<span data-ttu-id="095fc-155">Баннерная версия логотипа вашей компании, которая отображается на странице входного знака.</span><span class="sxs-lookup"><span data-stu-id="095fc-155">A banner version of your company logo that appears on the sign-in page.</span></span> <span data-ttu-id="095fc-156">Баннер — это .png или .jpg размером не более 36x245px.</span><span class="sxs-lookup"><span data-stu-id="095fc-156">The banner is a .png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="095fc-157">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="095fc-157">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="095fc-158">signInPageText</span><span class="sxs-lookup"><span data-stu-id="095fc-158">signInPageText</span></span>|<span data-ttu-id="095fc-159">String</span><span class="sxs-lookup"><span data-stu-id="095fc-159">String</span></span>|<span data-ttu-id="095fc-160">Текст, который отображается в нижней части окна для регистрации.</span><span class="sxs-lookup"><span data-stu-id="095fc-160">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="095fc-161">С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="095fc-161">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="095fc-162">Этот текст должен быть unicode и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="095fc-162">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="095fc-163">squareLogo</span><span class="sxs-lookup"><span data-stu-id="095fc-163">squareLogo</span></span>|<span data-ttu-id="095fc-164">Stream</span><span class="sxs-lookup"><span data-stu-id="095fc-164">Stream</span></span>|<span data-ttu-id="095fc-165">Квадратная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="095fc-165">Square version of your company logo.</span></span> <span data-ttu-id="095fc-166">Это отображается в windows 10 вне окна (OOBE) опытом и когда Windows Автопилот включен для развертывания.</span><span class="sxs-lookup"><span data-stu-id="095fc-166">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="095fc-167">Логотип — это .png или .jpg размером не более 240x240px и размером не более 10 кб.</span><span class="sxs-lookup"><span data-stu-id="095fc-167">The logo is a .png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="095fc-168">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="095fc-168">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="095fc-169">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="095fc-169">usernameHintText</span></span>|<span data-ttu-id="095fc-170">String</span><span class="sxs-lookup"><span data-stu-id="095fc-170">String</span></span>|<span data-ttu-id="095fc-171">Подсказка в текстовом ящике имени пользователя на экране входной записи.</span><span class="sxs-lookup"><span data-stu-id="095fc-171">The hint in the username textbox on the sign-in screen.</span></span> <span data-ttu-id="095fc-172">Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="095fc-172">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="095fc-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="095fc-173">Response</span></span>

<span data-ttu-id="095fc-174">В случае успешной работы этот метод возвращает код ответа и созданный `201 Created` [объект organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="095fc-174">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="095fc-175">Примеры</span><span class="sxs-lookup"><span data-stu-id="095fc-175">Examples</span></span>

<span data-ttu-id="095fc-176">В следующем примере создается брендинг по умолчанию и локализация **контент-языка.** `en-US`</span><span class="sxs-lookup"><span data-stu-id="095fc-176">The following example creates default branding and localization where **Content-Language** is `en-US`.</span></span>

### <a name="request"></a><span data-ttu-id="095fc-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="095fc-177">Request</span></span>

<span data-ttu-id="095fc-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="095fc-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```

### <a name="response"></a><span data-ttu-id="095fc-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="095fc-179">Response</span></span>

<span data-ttu-id="095fc-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="095fc-180">The following is an example of the response.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

<span data-ttu-id="095fc-181">В этом случае заданной является объект брендинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="095fc-181">In this case, the default branding object is set.</span></span> <span data-ttu-id="095fc-182">Локализованная торговая марка также устанавливается из-за загона Content-Language, даже несмотря на то, что набор брендинга не возвращается `en-US` в  `en-US` ответе.</span><span class="sxs-lookup"><span data-stu-id="095fc-182">Localized branding for `en-US` is also set due to the **Content-Language** header, even though the `en-US` branding set is not returned in the response.</span></span> <span data-ttu-id="095fc-183">**Заготвка Content-Language** в запросе необязательна, и если ее нет, она задает только брендинг по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="095fc-183">The **Content-Language** header in the request is optional, and if not present, only sets the default branding.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
