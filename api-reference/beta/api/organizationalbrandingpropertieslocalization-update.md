---
title: Обновление локализованных свойств организационногобрендинга
description: Обновление свойств объекта организационныхбрандингов для определенной локализации.
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c9c23e2ac73c35ad5d173dfbf524f30f6260d8e9
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679955"
---
# <a name="update-localized-organizationalbrandingproperties"></a><span data-ttu-id="e9089-103">Обновление локализованных свойств организационногобрендинга</span><span class="sxs-lookup"><span data-stu-id="e9089-103">Update Localized organizationalbrandingproperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9089-104">Обновление свойств объекта [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) для определенной локализации.</span><span class="sxs-lookup"><span data-stu-id="e9089-104">Update the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific localization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9089-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9089-105">Permissions</span></span>

<span data-ttu-id="e9089-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9089-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9089-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9089-108">Permission type</span></span>                        | <span data-ttu-id="e9089-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9089-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9089-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9089-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9089-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9089-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="e9089-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9089-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9089-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9089-113">Not supported.</span></span> |
| <span data-ttu-id="e9089-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9089-114">Application</span></span>                            | <span data-ttu-id="e9089-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9089-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9089-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9089-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{tenant id}/branding/localizations/{locale}
PUT /organization/{tenant id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="e9089-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9089-117">Request headers</span></span>

| <span data-ttu-id="e9089-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e9089-118">Name</span></span>       | <span data-ttu-id="e9089-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e9089-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e9089-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9089-120">Authorization</span></span> | <span data-ttu-id="e9089-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9089-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9089-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9089-123">Content-Type</span></span>  | <span data-ttu-id="e9089-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9089-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="e9089-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="e9089-126">Content-Language</span></span>  | <span data-ttu-id="e9089-127">Locale.</span><span class="sxs-lookup"><span data-stu-id="e9089-127">Locale.</span></span> <span data-ttu-id="e9089-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e9089-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9089-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9089-129">Request body</span></span>

<span data-ttu-id="e9089-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e9089-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e9089-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e9089-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e9089-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e9089-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e9089-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9089-133">Property</span></span>     | <span data-ttu-id="e9089-134">Тип</span><span class="sxs-lookup"><span data-stu-id="e9089-134">Type</span></span>        | <span data-ttu-id="e9089-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e9089-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9089-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="e9089-136">backgroundColor</span></span>|<span data-ttu-id="e9089-137">String</span><span class="sxs-lookup"><span data-stu-id="e9089-137">String</span></span>|<span data-ttu-id="e9089-138">Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="e9089-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="e9089-139">Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации.</span><span class="sxs-lookup"><span data-stu-id="e9089-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="e9089-140">Укажите это в hexadecimal (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="e9089-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="e9089-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="e9089-141">backgroundImage</span></span>|<span data-ttu-id="e9089-142">Stream</span><span class="sxs-lookup"><span data-stu-id="e9089-142">Stream</span></span>|<span data-ttu-id="e9089-143">Изображение, которое отображается в качестве фона знака на странице.</span><span class="sxs-lookup"><span data-stu-id="e9089-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="e9089-144">.png или .jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="e9089-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="e9089-145">Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.</span><span class="sxs-lookup"><span data-stu-id="e9089-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="e9089-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="e9089-146">bannerLogo</span></span>|<span data-ttu-id="e9089-147">Stream</span><span class="sxs-lookup"><span data-stu-id="e9089-147">Stream</span></span>|<span data-ttu-id="e9089-148">На странице входного знака отображается баннерная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="e9089-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="e9089-149">.png или .jpg не превышает 36x245px.</span><span class="sxs-lookup"><span data-stu-id="e9089-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="e9089-150">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="e9089-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="e9089-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="e9089-151">signInPageText</span></span>|<span data-ttu-id="e9089-152">String</span><span class="sxs-lookup"><span data-stu-id="e9089-152">String</span></span>|<span data-ttu-id="e9089-153">Текст, который отображается в нижней части окна для регистрации.</span><span class="sxs-lookup"><span data-stu-id="e9089-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="e9089-154">С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="e9089-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="e9089-155">Этот текст должен быть unicode и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="e9089-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="e9089-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="e9089-156">squareLogo</span></span>|<span data-ttu-id="e9089-157">Stream</span><span class="sxs-lookup"><span data-stu-id="e9089-157">Stream</span></span>|<span data-ttu-id="e9089-158">Квадратная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="e9089-158">Square version of your company logo.</span></span> <span data-ttu-id="e9089-159">Это отображается в Windows 10(OOBE) и когда Windows автопилот включен для развертывания.</span><span class="sxs-lookup"><span data-stu-id="e9089-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="e9089-160">.png или .jpg размером не более 240x240px и не более 10 кб.</span><span class="sxs-lookup"><span data-stu-id="e9089-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="e9089-161">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="e9089-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="e9089-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="e9089-162">usernameHintText</span></span>|<span data-ttu-id="e9089-163">String</span><span class="sxs-lookup"><span data-stu-id="e9089-163">String</span></span>|<span data-ttu-id="e9089-164">Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране знака.</span><span class="sxs-lookup"><span data-stu-id="e9089-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="e9089-165">Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="e9089-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="e9089-166">id</span><span class="sxs-lookup"><span data-stu-id="e9089-166">id</span></span>|<span data-ttu-id="e9089-167">String</span><span class="sxs-lookup"><span data-stu-id="e9089-167">String</span></span>|<span data-ttu-id="e9089-168">Locale для обновления брендинга для</span><span class="sxs-lookup"><span data-stu-id="e9089-168">Locale to update branding for</span></span>|


## <a name="response"></a><span data-ttu-id="e9089-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9089-169">Response</span></span>

<span data-ttu-id="e9089-170">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="e9089-170">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e9089-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="e9089-171">Examples</span></span>

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a><span data-ttu-id="e9089-172">Пример 1. Настройка **bannerLogo** для локализации fr с помощью PUT</span><span class="sxs-lookup"><span data-stu-id="e9089-172">Example 1: Setting **bannerLogo** for the fr localization using PUT</span></span>

<span data-ttu-id="e9089-173">Следующий запрос обновляет логотип баннера для локализации fr.</span><span class="sxs-lookup"><span data-stu-id="e9089-173">The following request updates the banner logo for the fr localization.</span></span> <span data-ttu-id="e9089-174">С помощью PUT, если локализация fr не существует, возвращается "404 не найден".</span><span class="sxs-lookup"><span data-stu-id="e9089-174">Using PUT, if the fr localization does not exist, "404 not found" is returned.</span></span> <span data-ttu-id="e9089-175">Если в полезной нагрузке содержится свойство id или заглавное свойство Content-Language и они не совпадают с id в URL-адресе, возвращается плохой запрос.</span><span class="sxs-lookup"><span data-stu-id="e9089-175">If the payload contains an id property or Content-Language header, and they don't match id in URL, a Bad Request is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="e9089-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9089-176">Request</span></span>

<span data-ttu-id="e9089-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9089-177">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9089-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9089-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_5"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[<span data-ttu-id="e9089-179">C#</span><span class="sxs-lookup"><span data-stu-id="e9089-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9089-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9089-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9089-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9089-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9089-182">Java</span><span class="sxs-lookup"><span data-stu-id="e9089-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9089-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9089-183">Response</span></span>

<span data-ttu-id="e9089-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9089-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a><span data-ttu-id="e9089-185">Пример 2. Обновление **bannerLogo** для локализации fr с помощью PATCH</span><span class="sxs-lookup"><span data-stu-id="e9089-185">Example 2: Update **bannerLogo** for the fr localization using PATCH</span></span>

<span data-ttu-id="e9089-186">Следующий запрос обновляет логотип баннера для локализации fr.</span><span class="sxs-lookup"><span data-stu-id="e9089-186">The following request updates the banner logo for the fr localization.</span></span>  <span data-ttu-id="e9089-187">С помощью PATCH, если указанная локализация еще не существует, она создается и свойство записано на него.</span><span class="sxs-lookup"><span data-stu-id="e9089-187">Using PATCH, if the specified localization does not already exist, it is created and the property is written to it.</span></span>

#### <a name="request"></a><span data-ttu-id="e9089-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9089-188">Request</span></span>

<span data-ttu-id="e9089-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9089-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9089-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9089-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_6"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="e9089-191">C#</span><span class="sxs-lookup"><span data-stu-id="e9089-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9089-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9089-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9089-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9089-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9089-194">Java</span><span class="sxs-lookup"><span data-stu-id="e9089-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9089-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9089-195">Response</span></span>
<span data-ttu-id="e9089-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9089-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a><span data-ttu-id="e9089-197">Пример 3. Переопределение значения брендинга по умолчанию с пустой строкой</span><span class="sxs-lookup"><span data-stu-id="e9089-197">Example 3: Override default branding value with a blank string</span></span>

<span data-ttu-id="e9089-198">Если значение свойства в локализации является null, это значение будет унаследовано от фирменного бренда по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e9089-198">If the value of a property in a localization is null, the value will be inherited from the default branding.</span></span> <span data-ttu-id="e9089-199">Чтобы этого не произошло, установите пустую строку или строку, содержащую только белое пространство в локализованной фирме.</span><span class="sxs-lookup"><span data-stu-id="e9089-199">To prevent this from happening, set an empty string or string containing only whitespace in the localized branding.</span></span>

#### <a name="request"></a><span data-ttu-id="e9089-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9089-200">Request</span></span>

<span data-ttu-id="e9089-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9089-201">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_7"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a><span data-ttu-id="e9089-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9089-202">Response</span></span>

<span data-ttu-id="e9089-203">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9089-203">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="e9089-204">После этого запроса имя пользователяHintText для локализации fr будет пустым, а не наследуется значение от брендинга по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e9089-204">Following this request, usernameHintText for the fr localization will be empty instead of inheriting the value from default branding.</span></span>

### <a name="example-4-replace-french-localization-with-put"></a><span data-ttu-id="e9089-205">Пример 4. Замена французской локализации на PUT</span><span class="sxs-lookup"><span data-stu-id="e9089-205">Example 4: Replace French localization with PUT</span></span>

<span data-ttu-id="e9089-206">Чтобы сделать обновление по локализации с помощью PUT, мы должны добавить все свойства в теле вместе с свойством, которое необходимо обновить по мере замены существующего объекта на новый.</span><span class="sxs-lookup"><span data-stu-id="e9089-206">To make an update on localization using PUT, we should add all properties in body along with the property that needs to be updated as PUT replaces existing object with the new one.</span></span> <span data-ttu-id="e9089-207">Другие свойства, которые не находятся в теле полезной нагрузки PUT, будут настроены на NULL.</span><span class="sxs-lookup"><span data-stu-id="e9089-207">The other properties which are not in the payload body of PUT will be set to NULL.</span></span> <span data-ttu-id="e9089-208">В приведенном ниже примере сохраняется только свойство backgroundColor и обновляется signInPageText, в то время как для других установлено null.</span><span class="sxs-lookup"><span data-stu-id="e9089-208">Here in example below, only backgroundColor property is retained and signInPageText is updated while others are set to null.</span></span>
<span data-ttu-id="e9089-209">Если указанная локализация еще не существует, ВСТАВЬТЕ в URL-адрес с указанием, что локализация создает ее.</span><span class="sxs-lookup"><span data-stu-id="e9089-209">If the specified localization does not already exist, PUT to the URL specifying that localization creates it.</span></span>
<span data-ttu-id="e9089-210">Если в полезной нагрузке содержится свойство id или заглавное свойство Content-Language, и они не совпадают с id в URL-адресе, мы бросаем плохой запрос.</span><span class="sxs-lookup"><span data-stu-id="e9089-210">If the payload contains an id property or a Content-Language header, and they don't match id in URL, we throw Bad request.</span></span>

#### <a name="request"></a><span data-ttu-id="e9089-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9089-211">Request</span></span>

<span data-ttu-id="e9089-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9089-212">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9089-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9089-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_8"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="e9089-214">C#</span><span class="sxs-lookup"><span data-stu-id="e9089-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-8-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9089-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9089-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-8-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9089-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9089-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-8-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9089-217">Java</span><span class="sxs-lookup"><span data-stu-id="e9089-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-8-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e9089-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9089-218">Response</span></span>
<span data-ttu-id="e9089-219">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e9089-219">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
