---
title: Обновление организационных свойств
description: Обновление свойств объекта organizationalBrandingProperties.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f6b1d4327ce036f9623d4ad62aa0d872746eb20f
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582811"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="15bd3-103">Обновление организационных свойств</span><span class="sxs-lookup"><span data-stu-id="15bd3-103">Update organizationalBrandingProperties</span></span>

<span data-ttu-id="15bd3-104">Обновление свойств объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="15bd3-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="15bd3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15bd3-105">Permissions</span></span>

<span data-ttu-id="15bd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15bd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15bd3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15bd3-108">Permission type</span></span>                        | <span data-ttu-id="15bd3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15bd3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="15bd3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15bd3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="15bd3-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15bd3-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="15bd3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15bd3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15bd3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15bd3-113">Not supported.</span></span> |
| <span data-ttu-id="15bd3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15bd3-114">Application</span></span>                            | <span data-ttu-id="15bd3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15bd3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="15bd3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15bd3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="15bd3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15bd3-117">Request headers</span></span>

| <span data-ttu-id="15bd3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="15bd3-118">Name</span></span>       | <span data-ttu-id="15bd3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="15bd3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="15bd3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15bd3-120">Authorization</span></span> | <span data-ttu-id="15bd3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15bd3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15bd3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15bd3-123">Content-Type</span></span>  | <span data-ttu-id="15bd3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15bd3-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="15bd3-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="15bd3-126">Content-Language</span></span>  | <span data-ttu-id="15bd3-127">Locale.</span><span class="sxs-lookup"><span data-stu-id="15bd3-127">Locale.</span></span> <span data-ttu-id="15bd3-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="15bd3-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15bd3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15bd3-129">Request body</span></span>

<span data-ttu-id="15bd3-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="15bd3-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="15bd3-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="15bd3-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="15bd3-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="15bd3-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="15bd3-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="15bd3-133">Property</span></span>     | <span data-ttu-id="15bd3-134">Тип</span><span class="sxs-lookup"><span data-stu-id="15bd3-134">Type</span></span>        | <span data-ttu-id="15bd3-135">Описание</span><span class="sxs-lookup"><span data-stu-id="15bd3-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="15bd3-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="15bd3-136">backgroundColor</span></span>|<span data-ttu-id="15bd3-137">String</span><span class="sxs-lookup"><span data-stu-id="15bd3-137">String</span></span>|<span data-ttu-id="15bd3-138">Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="15bd3-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="15bd3-139">Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации.</span><span class="sxs-lookup"><span data-stu-id="15bd3-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="15bd3-140">Укажите это в hexadecimal (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="15bd3-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="15bd3-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="15bd3-141">backgroundImage</span></span>|<span data-ttu-id="15bd3-142">Stream</span><span class="sxs-lookup"><span data-stu-id="15bd3-142">Stream</span></span>|<span data-ttu-id="15bd3-143">Изображение, которое отображается в качестве фона знака на странице.</span><span class="sxs-lookup"><span data-stu-id="15bd3-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="15bd3-144">.png или .jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="15bd3-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="15bd3-145">Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.</span><span class="sxs-lookup"><span data-stu-id="15bd3-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="15bd3-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="15bd3-146">bannerLogo</span></span>|<span data-ttu-id="15bd3-147">Stream</span><span class="sxs-lookup"><span data-stu-id="15bd3-147">Stream</span></span>|<span data-ttu-id="15bd3-148">На странице входного знака отображается баннерная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="15bd3-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="15bd3-149">.png или .jpg не больше 36x245px.</span><span class="sxs-lookup"><span data-stu-id="15bd3-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="15bd3-150">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="15bd3-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="15bd3-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="15bd3-151">signInPageText</span></span>|<span data-ttu-id="15bd3-152">String</span><span class="sxs-lookup"><span data-stu-id="15bd3-152">String</span></span>|<span data-ttu-id="15bd3-153">Текст, который отображается в нижней части окна для регистрации.</span><span class="sxs-lookup"><span data-stu-id="15bd3-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="15bd3-154">С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="15bd3-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="15bd3-155">Этот текст должен быть unicode и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="15bd3-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="15bd3-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="15bd3-156">squareLogo</span></span>|<span data-ttu-id="15bd3-157">Stream</span><span class="sxs-lookup"><span data-stu-id="15bd3-157">Stream</span></span>|<span data-ttu-id="15bd3-158">Квадратная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="15bd3-158">Square version of your company logo.</span></span> <span data-ttu-id="15bd3-159">Это отображается в windows 10 вне окна (OOBE) опытом и когда Windows Автопилот включен для развертывания.</span><span class="sxs-lookup"><span data-stu-id="15bd3-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="15bd3-160">.png или .jpg размером не более 240x240px и размером не более 10 кб.</span><span class="sxs-lookup"><span data-stu-id="15bd3-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="15bd3-161">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="15bd3-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="15bd3-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="15bd3-162">usernameHintText</span></span>|<span data-ttu-id="15bd3-163">String</span><span class="sxs-lookup"><span data-stu-id="15bd3-163">String</span></span>|<span data-ttu-id="15bd3-164">Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране знака.</span><span class="sxs-lookup"><span data-stu-id="15bd3-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="15bd3-165">Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="15bd3-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="15bd3-166">Свойство **id** игнорируется при проходе.</span><span class="sxs-lookup"><span data-stu-id="15bd3-166">The **id** property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="15bd3-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="15bd3-167">Response</span></span>

<span data-ttu-id="15bd3-168">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="15bd3-168">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="15bd3-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="15bd3-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="15bd3-170">Пример 1. Обновление брандминга по умолчанию</span><span class="sxs-lookup"><span data-stu-id="15bd3-170">Example 1: Update default branding</span></span>
<span data-ttu-id="15bd3-171">Если брендинг уже существует, заменит только указанные свойства, оставив `PATCH` неустановленные свойства без изменений.</span><span class="sxs-lookup"><span data-stu-id="15bd3-171">If the branding already exists, `PATCH` will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="15bd3-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="15bd3-172">Request</span></span>

<span data-ttu-id="15bd3-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15bd3-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="15bd3-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="15bd3-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_1"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[<span data-ttu-id="15bd3-175">C#</span><span class="sxs-lookup"><span data-stu-id="15bd3-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15bd3-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15bd3-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15bd3-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15bd3-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15bd3-178">Java</span><span class="sxs-lookup"><span data-stu-id="15bd3-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="15bd3-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="15bd3-179">Response</span></span>
<span data-ttu-id="15bd3-180">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="15bd3-180">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="15bd3-181">В этом случае значения брендинга по умолчанию обновляются, но никакие значения не меняются при любой локализации.</span><span class="sxs-lookup"><span data-stu-id="15bd3-181">In this case, the values of the default branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="15bd3-182">Пример 2. Обновление bannerLogo для брендинга по умолчанию</span><span class="sxs-lookup"><span data-stu-id="15bd3-182">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="15bd3-183">Следующий запрос обновляет логотип баннера для фирменого знака по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="15bd3-183">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="15bd3-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="15bd3-184">Request</span></span>

<span data-ttu-id="15bd3-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15bd3-185">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="15bd3-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="15bd3-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_2"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="15bd3-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="15bd3-187">Response</span></span>
<span data-ttu-id="15bd3-188">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="15bd3-188">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="15bd3-189">Пример 3. Обновление локализованного брендинга</span><span class="sxs-lookup"><span data-stu-id="15bd3-189">Example 3: Update localized branding</span></span>
<span data-ttu-id="15bd3-190">Если **заглавное** заглавье content-Language задано, локализация, связанная с **Content-Language,** сначала создается, если она еще не существует, а затем обновляется с помощью указанных значений.</span><span class="sxs-lookup"><span data-stu-id="15bd3-190">If **Content-Language** header is specified, the localization associated with **Content-Language** is first created if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="15bd3-191">Брендинг по умолчанию не меняется.</span><span class="sxs-lookup"><span data-stu-id="15bd3-191">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="15bd3-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="15bd3-192">Request</span></span>

<span data-ttu-id="15bd3-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15bd3-193">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_3"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="15bd3-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="15bd3-194">Response</span></span>
<span data-ttu-id="15bd3-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="15bd3-195">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="15bd3-196">После этого запроса локализация обновляется с новым значением backgroundColor, но в брандминг по умолчанию не `fr` меняется. </span><span class="sxs-lookup"><span data-stu-id="15bd3-196">Following this request, the `fr` localization is updated with the new value of **backgroundColor**, but no change is made to the default branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="15bd3-197">Пример 4. Замена брендинга по умолчанию и всех локализации</span><span class="sxs-lookup"><span data-stu-id="15bd3-197">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="15bd3-198">Если брендинг уже существует, заменит брендинг по умолчанию `PUT` и любые локализации.</span><span class="sxs-lookup"><span data-stu-id="15bd3-198">If the branding already exists, `PUT` will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="15bd3-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="15bd3-199">Request</span></span>

<span data-ttu-id="15bd3-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15bd3-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="15bd3-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="15bd3-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_4"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```
# <a name="c"></a>[<span data-ttu-id="15bd3-202">C#</span><span class="sxs-lookup"><span data-stu-id="15bd3-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15bd3-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15bd3-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15bd3-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15bd3-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15bd3-205">Java</span><span class="sxs-lookup"><span data-stu-id="15bd3-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="15bd3-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="15bd3-206">Response</span></span>
<span data-ttu-id="15bd3-207">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="15bd3-207">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="15bd3-208">После этого запроса брендинг по умолчанию имеет только **указанный backgroundColor** и имеет точно одну локализацию с **id,** также `fr` с **набором backgroundColor.**</span><span class="sxs-lookup"><span data-stu-id="15bd3-208">Following this request, the default branding has only the **backgroundColor** specified and has exactly one localization with the **id** `fr`, also with the **backgroundColor** set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
