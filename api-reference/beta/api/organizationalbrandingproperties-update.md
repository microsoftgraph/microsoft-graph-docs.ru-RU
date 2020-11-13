---
title: Обновление Организатионалбрандингпропертиес
description: Обновление свойств объекта Организатионалбрандингпропертиес.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7655caa6e5c8eb1187bcc159f7f6d8c78641abc9
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031979"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="6c9e2-103">Обновление Организатионалбрандингпропертиес</span><span class="sxs-lookup"><span data-stu-id="6c9e2-103">Update organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c9e2-104">Обновление свойств объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="6c9e2-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c9e2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c9e2-105">Permissions</span></span>

<span data-ttu-id="6c9e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c9e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c9e2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c9e2-108">Permission type</span></span>                        | <span data-ttu-id="6c9e2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c9e2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c9e2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c9e2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c9e2-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c9e2-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="6c9e2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c9e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c9e2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-113">Not supported.</span></span> |
| <span data-ttu-id="6c9e2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c9e2-114">Application</span></span>                            | <span data-ttu-id="6c9e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c9e2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c9e2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="6c9e2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c9e2-117">Request headers</span></span>

| <span data-ttu-id="6c9e2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6c9e2-118">Name</span></span>       | <span data-ttu-id="6c9e2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6c9e2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6c9e2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c9e2-120">Authorization</span></span> | <span data-ttu-id="6c9e2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c9e2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c9e2-123">Content-Type</span></span>  | <span data-ttu-id="6c9e2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="6c9e2-126">Content — Language</span><span class="sxs-lookup"><span data-stu-id="6c9e2-126">Content-Language</span></span>  | <span data-ttu-id="6c9e2-127">Языковой стандарт.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-127">Locale.</span></span> <span data-ttu-id="6c9e2-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c9e2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c9e2-129">Request body</span></span>

<span data-ttu-id="6c9e2-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6c9e2-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6c9e2-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6c9e2-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c9e2-133">Property</span></span>     | <span data-ttu-id="6c9e2-134">Тип</span><span class="sxs-lookup"><span data-stu-id="6c9e2-134">Type</span></span>        | <span data-ttu-id="6c9e2-135">Описание</span><span class="sxs-lookup"><span data-stu-id="6c9e2-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c9e2-136">баккграундколор</span><span class="sxs-lookup"><span data-stu-id="6c9e2-136">backgroundColor</span></span>|<span data-ttu-id="6c9e2-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6c9e2-137">String</span></span>|<span data-ttu-id="6c9e2-138">Цвет, который будет отображаться вместо фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="6c9e2-139">Рекомендуется использовать основной цвет эмблемы баннера или цвет вашей организации.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="6c9e2-140">Укажите в шестнадцатеричном формате (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="6c9e2-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="6c9e2-141">Изображение</span><span class="sxs-lookup"><span data-stu-id="6c9e2-141">backgroundImage</span></span>|<span data-ttu-id="6c9e2-142">Stream</span><span class="sxs-lookup"><span data-stu-id="6c9e2-142">Stream</span></span>|<span data-ttu-id="6c9e2-143">Изображение, отображаемое в качестве фона страницы входа.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="6c9e2-144">файлы PNG или jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="6c9e2-145">Изображение меньшего размера уменьшит требования к пропускной способности и сделает загрузку страниц более производительной.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="6c9e2-146">баннерлого</span><span class="sxs-lookup"><span data-stu-id="6c9e2-146">bannerLogo</span></span>|<span data-ttu-id="6c9e2-147">Stream</span><span class="sxs-lookup"><span data-stu-id="6c9e2-147">Stream</span></span>|<span data-ttu-id="6c9e2-148">На странице входа отображается плакатная эмблема компании.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="6c9e2-149">файлы PNG или jpg не больше 36x245px.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="6c9e2-150">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="6c9e2-151">сигнинпажетекст</span><span class="sxs-lookup"><span data-stu-id="6c9e2-151">signInPageText</span></span>|<span data-ttu-id="6c9e2-152">Строка</span><span class="sxs-lookup"><span data-stu-id="6c9e2-152">String</span></span>|<span data-ttu-id="6c9e2-153">Текст, который отображается в нижней части поля входа.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="6c9e2-154">Вы можете использовать эту возможность для передачи дополнительных сведений, таких как номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="6c9e2-155">Этот текст должен быть Юникодом и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="6c9e2-156">скуарелого</span><span class="sxs-lookup"><span data-stu-id="6c9e2-156">squareLogo</span></span>|<span data-ttu-id="6c9e2-157">Stream</span><span class="sxs-lookup"><span data-stu-id="6c9e2-157">Stream</span></span>|<span data-ttu-id="6c9e2-158">Квадратная версия логотипа компании.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-158">Square version of your company logo.</span></span> <span data-ttu-id="6c9e2-159">Эта функция отображается в режиме готовности к работе с Windows 10 (OOBE) и при включенном развертывании Windows.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="6c9e2-160">файлы PNG или jpg не имеют размер больше 240x240px и не больше 10Kb.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="6c9e2-161">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="6c9e2-162">усернамехинттекст</span><span class="sxs-lookup"><span data-stu-id="6c9e2-162">usernameHintText</span></span>|<span data-ttu-id="6c9e2-163">Строка</span><span class="sxs-lookup"><span data-stu-id="6c9e2-163">String</span></span>|<span data-ttu-id="6c9e2-164">Строка, которая отображается как подсказка в текстовом поле имя пользователя на экране входа.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="6c9e2-165">Этот текст должен быть Юникодом без ссылок или кода и не может содержать более 64 символов.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="6c9e2-166">Свойство **ID** игнорируется при передаче.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-166">The **id** property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="6c9e2-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c9e2-167">Response</span></span>

<span data-ttu-id="6c9e2-168">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-168">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6c9e2-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c9e2-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="6c9e2-170">Пример 1: обновление фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6c9e2-170">Example 1: Update default branding</span></span>
<span data-ttu-id="6c9e2-171">Если фирменная символика уже существует, то функция PATCH заменяет только указанные свойства, оставляя неопределенные свойства без изменений.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-171">If the branding already exists, PATCH will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="6c9e2-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c9e2-172">Request</span></span>

<span data-ttu-id="6c9e2-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-173">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

#### <a name="response"></a><span data-ttu-id="6c9e2-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c9e2-174">Response</span></span>
<span data-ttu-id="6c9e2-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="6c9e2-176">В этом случае значения/брандинг по умолчанию обновляются, но при локализации значения не изменяются.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-176">In this case, the values of the default /branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="6c9e2-177">Пример 2: Update Баннерлого для фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6c9e2-177">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="6c9e2-178">Следующий запрос обновляет логотип баннера для фирменной символики по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-178">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="6c9e2-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c9e2-179">Request</span></span>

<span data-ttu-id="6c9e2-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-180">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="6c9e2-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c9e2-181">Response</span></span>
<span data-ttu-id="6c9e2-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-182">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="6c9e2-183">Пример 3: обновление локализованной фирменной символики</span><span class="sxs-lookup"><span data-stu-id="6c9e2-183">Example 3: Update localized branding</span></span>
<span data-ttu-id="6c9e2-184">Если указан заголовок Content-Language, создается локализация, связанная с языком содержимого, если она еще не существует, а затем она обновляется с использованием указанных значений.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-184">If Content-Language header is specified the localization associated with Content-Language is created, if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="6c9e2-185">Фирменная символика по умолчанию не изменяется.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-185">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="6c9e2-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c9e2-186">Request</span></span>

<span data-ttu-id="6c9e2-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-187">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="6c9e2-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c9e2-188">Response</span></span>
<span data-ttu-id="6c9e2-189">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-189">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="6c9e2-190">После этого запроса локализация fr обновляется новым значением Баккграундколор, но в/брандинг. по умолчанию не вносятся изменения.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-190">Following this request, the fr localization is updated with the new value of backgroundColor, but no change is made to the default /branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="6c9e2-191">Пример 4: замена фирменного стиля по умолчанию и всех локализаций</span><span class="sxs-lookup"><span data-stu-id="6c9e2-191">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="6c9e2-192">Если фирменная символика уже существует, при РАЗМЕЩЕНии будут заменены фирменные настройки по умолчанию и все локализации.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-192">If the branding already exists, PUT will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="6c9e2-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c9e2-193">Request</span></span>

<span data-ttu-id="6c9e2-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-194">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="6c9e2-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c9e2-195">Response</span></span>
<span data-ttu-id="6c9e2-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="6c9e2-197">В соответствии с этим запросом фирменная символика по умолчанию имеет только указанный Баккграундколор и имеет только одну локализацию с идентификатором fr, а также набор Баккграундколор.</span><span class="sxs-lookup"><span data-stu-id="6c9e2-197">Following this request, the default branding has only the backgroundColor specified and has exactly one localization with the id fr, also with the backgroundColor set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
