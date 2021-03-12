---
title: Обновление организационных свойств
description: Обновление свойств объекта organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1fd15c3ae41af043cb7c5163d8b7ac8b06a36ae0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722646"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="e8864-103">Обновление организационных свойств</span><span class="sxs-lookup"><span data-stu-id="e8864-103">Update organizationalBrandingProperties</span></span>

<span data-ttu-id="e8864-104">Обновление свойств объекта [organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="e8864-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8864-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8864-105">Permissions</span></span>

<span data-ttu-id="e8864-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8864-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8864-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8864-108">Permission type</span></span>                        | <span data-ttu-id="e8864-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8864-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8864-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8864-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8864-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8864-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="e8864-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8864-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8864-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8864-113">Not supported.</span></span> |
| <span data-ttu-id="e8864-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8864-114">Application</span></span>                            | <span data-ttu-id="e8864-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8864-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8864-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8864-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="e8864-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8864-117">Request headers</span></span>

| <span data-ttu-id="e8864-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e8864-118">Name</span></span>       | <span data-ttu-id="e8864-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e8864-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e8864-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8864-120">Authorization</span></span> | <span data-ttu-id="e8864-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8864-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8864-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8864-123">Content-Type</span></span>  | <span data-ttu-id="e8864-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8864-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="e8864-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="e8864-126">Content-Language</span></span>  | <span data-ttu-id="e8864-127">Locale.</span><span class="sxs-lookup"><span data-stu-id="e8864-127">Locale.</span></span> <span data-ttu-id="e8864-128">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="e8864-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8864-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8864-129">Request body</span></span>

<span data-ttu-id="e8864-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e8864-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e8864-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e8864-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e8864-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e8864-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e8864-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8864-133">Property</span></span>     | <span data-ttu-id="e8864-134">Тип</span><span class="sxs-lookup"><span data-stu-id="e8864-134">Type</span></span>        | <span data-ttu-id="e8864-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e8864-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e8864-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="e8864-136">backgroundColor</span></span>|<span data-ttu-id="e8864-137">String</span><span class="sxs-lookup"><span data-stu-id="e8864-137">String</span></span>|<span data-ttu-id="e8864-138">Цвет, который будет отображаться на месте фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="e8864-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="e8864-139">Здесь рекомендуется использовать основной цвет логотипа баннера или цвета организации.</span><span class="sxs-lookup"><span data-stu-id="e8864-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="e8864-140">Укажите это в hexadecimal (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="e8864-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="e8864-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="e8864-141">backgroundImage</span></span>|<span data-ttu-id="e8864-142">Stream</span><span class="sxs-lookup"><span data-stu-id="e8864-142">Stream</span></span>|<span data-ttu-id="e8864-143">Изображение, которое отображается в качестве фона знака на странице.</span><span class="sxs-lookup"><span data-stu-id="e8864-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="e8864-144">.png или .jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="e8864-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="e8864-145">Меньшее изображение уменьшит требования к пропускной способности и сделает загрузку страниц более высокой.</span><span class="sxs-lookup"><span data-stu-id="e8864-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="e8864-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="e8864-146">bannerLogo</span></span>|<span data-ttu-id="e8864-147">Stream</span><span class="sxs-lookup"><span data-stu-id="e8864-147">Stream</span></span>|<span data-ttu-id="e8864-148">На странице входного знака отображается баннерная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="e8864-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="e8864-149">.png или .jpg не больше 36x245px.</span><span class="sxs-lookup"><span data-stu-id="e8864-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="e8864-150">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="e8864-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="e8864-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="e8864-151">signInPageText</span></span>|<span data-ttu-id="e8864-152">String</span><span class="sxs-lookup"><span data-stu-id="e8864-152">String</span></span>|<span data-ttu-id="e8864-153">Текст, который отображается в нижней части окна для регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8864-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="e8864-154">С помощью этого можно сообщить дополнительные сведения, например номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="e8864-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="e8864-155">Этот текст должен быть unicode и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="e8864-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="e8864-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="e8864-156">squareLogo</span></span>|<span data-ttu-id="e8864-157">Stream</span><span class="sxs-lookup"><span data-stu-id="e8864-157">Stream</span></span>|<span data-ttu-id="e8864-158">Квадратная версия логотипа вашей компании.</span><span class="sxs-lookup"><span data-stu-id="e8864-158">Square version of your company logo.</span></span> <span data-ttu-id="e8864-159">Это отображается в windows 10 вне окна (OOBE) опытом и когда Windows Автопилот включен для развертывания.</span><span class="sxs-lookup"><span data-stu-id="e8864-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="e8864-160">.png или .jpg размером не более 240x240px и размером не более 10 кб.</span><span class="sxs-lookup"><span data-stu-id="e8864-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="e8864-161">Рекомендуется использовать прозрачное изображение без обивки вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="e8864-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="e8864-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="e8864-162">usernameHintText</span></span>|<span data-ttu-id="e8864-163">String</span><span class="sxs-lookup"><span data-stu-id="e8864-163">String</span></span>|<span data-ttu-id="e8864-164">Строка, отображаемая в виде подсказки в текстовом ящике имени пользователя на экране знака.</span><span class="sxs-lookup"><span data-stu-id="e8864-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="e8864-165">Этот текст должен быть Unicode без ссылок или кода и не может превышать 64 символов.</span><span class="sxs-lookup"><span data-stu-id="e8864-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="e8864-166">Свойство `id` игнорируется при проходе.</span><span class="sxs-lookup"><span data-stu-id="e8864-166">The `id` property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="e8864-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8864-167">Response</span></span>

<span data-ttu-id="e8864-168">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e8864-168">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e8864-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="e8864-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="e8864-170">Пример 1. Обновление брандминга по умолчанию</span><span class="sxs-lookup"><span data-stu-id="e8864-170">Example 1: Update default branding</span></span>
<span data-ttu-id="e8864-171">Если брендинг уже существует, PATCH заменит только указанные свойства, оставив неустановленные свойства без изменений.</span><span class="sxs-lookup"><span data-stu-id="e8864-171">If the branding already exists, PATCH will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="e8864-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8864-172">Request</span></span>

<span data-ttu-id="e8864-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8864-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

#### <a name="response"></a><span data-ttu-id="e8864-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8864-174">Response</span></span>
<span data-ttu-id="e8864-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8864-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="e8864-176">В этом случае значения по умолчанию /брендинга обновляются, но никакие значения не меняются при любой локализации.</span><span class="sxs-lookup"><span data-stu-id="e8864-176">In this case, the values of the default /branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="e8864-177">Пример 2. Обновление bannerLogo для брендинга по умолчанию</span><span class="sxs-lookup"><span data-stu-id="e8864-177">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="e8864-178">Следующий запрос обновляет логотип баннера для фирменого знака по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e8864-178">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="e8864-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8864-179">Request</span></span>

<span data-ttu-id="e8864-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8864-180">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="e8864-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8864-181">Response</span></span>
<span data-ttu-id="e8864-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8864-182">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="e8864-183">Пример 3. Обновление локализованного брендинга</span><span class="sxs-lookup"><span data-stu-id="e8864-183">Example 3: Update localized branding</span></span>
<span data-ttu-id="e8864-184">Если заготвка Content-Language задана, создается локализация, связанная с Языком контента, если она еще не существует, а затем обновляется с помощью указанных значений.</span><span class="sxs-lookup"><span data-stu-id="e8864-184">If Content-Language header is specified the localization associated with Content-Language is created, if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="e8864-185">Брендинг по умолчанию не меняется.</span><span class="sxs-lookup"><span data-stu-id="e8864-185">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="e8864-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8864-186">Request</span></span>

<span data-ttu-id="e8864-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8864-187">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="e8864-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8864-188">Response</span></span>
<span data-ttu-id="e8864-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8864-189">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="e8864-190">После этого запроса локализация fr обновляется с новым значением backgroundColor, но не меняется значение по умолчанию /branding.</span><span class="sxs-lookup"><span data-stu-id="e8864-190">Following this request, the fr localization is updated with the new value of backgroundColor, but no change is made to the default /branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="e8864-191">Пример 4. Замена брендинга по умолчанию и всех локализации</span><span class="sxs-lookup"><span data-stu-id="e8864-191">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="e8864-192">Если брендинг уже существует, PUT заменит брендинг по умолчанию и любые локализации.</span><span class="sxs-lookup"><span data-stu-id="e8864-192">If the branding already exists, PUT will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="e8864-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8864-193">Request</span></span>

<span data-ttu-id="e8864-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8864-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="e8864-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8864-195">Response</span></span>
<span data-ttu-id="e8864-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8864-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="e8864-197">После этого запроса брендинг по умолчанию имеет только указанный фонColor и имеет точно одну локализацию с id fr, а также с набором backgroundColor.</span><span class="sxs-lookup"><span data-stu-id="e8864-197">Following this request, the default branding has only the backgroundColor specified and has exactly one localization with the id fr, also with the backgroundColor set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
