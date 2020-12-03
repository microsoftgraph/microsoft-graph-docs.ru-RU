---
title: Обновление Организатионалбрандингпропертиес
description: Обновление свойств объекта Организатионалбрандингпропертиес.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dd8eb2976fc3e8309f804714babbd45474574455
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524465"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="7e73d-103">Обновление Организатионалбрандингпропертиес</span><span class="sxs-lookup"><span data-stu-id="7e73d-103">Update organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e73d-104">Обновление свойств объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="7e73d-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e73d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e73d-105">Permissions</span></span>

<span data-ttu-id="7e73d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e73d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e73d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e73d-108">Permission type</span></span>                        | <span data-ttu-id="7e73d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e73d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e73d-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e73d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e73d-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e73d-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="7e73d-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e73d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e73d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e73d-113">Not supported.</span></span> |
| <span data-ttu-id="7e73d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e73d-114">Application</span></span>                            | <span data-ttu-id="7e73d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e73d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e73d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e73d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="7e73d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e73d-117">Request headers</span></span>

| <span data-ttu-id="7e73d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7e73d-118">Name</span></span>       | <span data-ttu-id="7e73d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7e73d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7e73d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e73d-120">Authorization</span></span> | <span data-ttu-id="7e73d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e73d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e73d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e73d-123">Content-Type</span></span>  | <span data-ttu-id="7e73d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e73d-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="7e73d-126">Content — Language</span><span class="sxs-lookup"><span data-stu-id="7e73d-126">Content-Language</span></span>  | <span data-ttu-id="7e73d-127">Языковой стандарт.</span><span class="sxs-lookup"><span data-stu-id="7e73d-127">Locale.</span></span> <span data-ttu-id="7e73d-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7e73d-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e73d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e73d-129">Request body</span></span>

<span data-ttu-id="7e73d-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="7e73d-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7e73d-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="7e73d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7e73d-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7e73d-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7e73d-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e73d-133">Property</span></span>     | <span data-ttu-id="7e73d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="7e73d-134">Type</span></span>        | <span data-ttu-id="7e73d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="7e73d-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7e73d-136">баккграундколор</span><span class="sxs-lookup"><span data-stu-id="7e73d-136">backgroundColor</span></span>|<span data-ttu-id="7e73d-137">String</span><span class="sxs-lookup"><span data-stu-id="7e73d-137">String</span></span>|<span data-ttu-id="7e73d-138">Цвет, который будет отображаться вместо фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="7e73d-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="7e73d-139">Рекомендуется использовать основной цвет эмблемы баннера или цвет вашей организации.</span><span class="sxs-lookup"><span data-stu-id="7e73d-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="7e73d-140">Укажите в шестнадцатеричном формате (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="7e73d-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="7e73d-141">Изображение</span><span class="sxs-lookup"><span data-stu-id="7e73d-141">backgroundImage</span></span>|<span data-ttu-id="7e73d-142">Stream</span><span class="sxs-lookup"><span data-stu-id="7e73d-142">Stream</span></span>|<span data-ttu-id="7e73d-143">Изображение, отображаемое в качестве фона страницы входа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="7e73d-144">файлы PNG или jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="7e73d-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="7e73d-145">Изображение меньшего размера уменьшит требования к пропускной способности и сделает загрузку страниц более производительной.</span><span class="sxs-lookup"><span data-stu-id="7e73d-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="7e73d-146">баннерлого</span><span class="sxs-lookup"><span data-stu-id="7e73d-146">bannerLogo</span></span>|<span data-ttu-id="7e73d-147">Stream</span><span class="sxs-lookup"><span data-stu-id="7e73d-147">Stream</span></span>|<span data-ttu-id="7e73d-148">На странице входа отображается плакатная эмблема компании.</span><span class="sxs-lookup"><span data-stu-id="7e73d-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="7e73d-149">файлы PNG или jpg не больше 36x245px.</span><span class="sxs-lookup"><span data-stu-id="7e73d-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="7e73d-150">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="7e73d-151">сигнинпажетекст</span><span class="sxs-lookup"><span data-stu-id="7e73d-151">signInPageText</span></span>|<span data-ttu-id="7e73d-152">String</span><span class="sxs-lookup"><span data-stu-id="7e73d-152">String</span></span>|<span data-ttu-id="7e73d-153">Текст, который отображается в нижней части поля входа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="7e73d-154">Вы можете использовать эту возможность для передачи дополнительных сведений, таких как номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="7e73d-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="7e73d-155">Этот текст должен быть Юникодом и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="7e73d-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="7e73d-156">скуарелого</span><span class="sxs-lookup"><span data-stu-id="7e73d-156">squareLogo</span></span>|<span data-ttu-id="7e73d-157">Stream</span><span class="sxs-lookup"><span data-stu-id="7e73d-157">Stream</span></span>|<span data-ttu-id="7e73d-158">Квадратная версия логотипа компании.</span><span class="sxs-lookup"><span data-stu-id="7e73d-158">Square version of your company logo.</span></span> <span data-ttu-id="7e73d-159">Эта функция отображается в режиме готовности к работе с Windows 10 (OOBE) и при включенном развертывании Windows.</span><span class="sxs-lookup"><span data-stu-id="7e73d-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="7e73d-160">файлы PNG или jpg не имеют размер больше 240x240px и не больше 10Kb.</span><span class="sxs-lookup"><span data-stu-id="7e73d-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="7e73d-161">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="7e73d-162">усернамехинттекст</span><span class="sxs-lookup"><span data-stu-id="7e73d-162">usernameHintText</span></span>|<span data-ttu-id="7e73d-163">String</span><span class="sxs-lookup"><span data-stu-id="7e73d-163">String</span></span>|<span data-ttu-id="7e73d-164">Строка, которая отображается как подсказка в текстовом поле имя пользователя на экране входа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="7e73d-165">Этот текст должен быть Юникодом без ссылок или кода и не может содержать более 64 символов.</span><span class="sxs-lookup"><span data-stu-id="7e73d-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="7e73d-166">Свойство **ID** игнорируется при передаче.</span><span class="sxs-lookup"><span data-stu-id="7e73d-166">The **id** property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="7e73d-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e73d-167">Response</span></span>

<span data-ttu-id="7e73d-168">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="7e73d-168">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7e73d-169">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e73d-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="7e73d-170">Пример 1: обновление фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="7e73d-170">Example 1: Update default branding</span></span>
<span data-ttu-id="7e73d-171">Если фирменная символика уже существует, то функция PATCH заменяет только указанные свойства, оставляя неопределенные свойства без изменений.</span><span class="sxs-lookup"><span data-stu-id="7e73d-171">If the branding already exists, PATCH will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="7e73d-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e73d-172">Request</span></span>

<span data-ttu-id="7e73d-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e73d-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e73d-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e73d-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7e73d-175">C#</span><span class="sxs-lookup"><span data-stu-id="7e73d-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e73d-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e73d-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e73d-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e73d-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e73d-178">Java</span><span class="sxs-lookup"><span data-stu-id="7e73d-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e73d-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e73d-179">Response</span></span>
<span data-ttu-id="7e73d-180">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-180">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="7e73d-181">В этом случае значения/брандинг по умолчанию обновляются, но при локализации значения не изменяются.</span><span class="sxs-lookup"><span data-stu-id="7e73d-181">In this case, the values of the default /branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="7e73d-182">Пример 2: Update Баннерлого для фирменной символики по умолчанию</span><span class="sxs-lookup"><span data-stu-id="7e73d-182">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="7e73d-183">Следующий запрос обновляет логотип баннера для фирменной символики по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7e73d-183">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="7e73d-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e73d-184">Request</span></span>

<span data-ttu-id="7e73d-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e73d-185">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e73d-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e73d-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[<span data-ttu-id="7e73d-187">C#</span><span class="sxs-lookup"><span data-stu-id="7e73d-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e73d-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e73d-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e73d-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e73d-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e73d-190">Java</span><span class="sxs-lookup"><span data-stu-id="7e73d-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e73d-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e73d-191">Response</span></span>
<span data-ttu-id="7e73d-192">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-192">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="7e73d-193">Пример 3: обновление локализованной фирменной символики</span><span class="sxs-lookup"><span data-stu-id="7e73d-193">Example 3: Update localized branding</span></span>
<span data-ttu-id="7e73d-194">Если указан заголовок Content-Language, создается локализация, связанная с языком содержимого, если она еще не существует, а затем она обновляется с использованием указанных значений.</span><span class="sxs-lookup"><span data-stu-id="7e73d-194">If Content-Language header is specified the localization associated with Content-Language is created, if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="7e73d-195">Фирменная символика по умолчанию не изменяется.</span><span class="sxs-lookup"><span data-stu-id="7e73d-195">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="7e73d-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e73d-196">Request</span></span>

<span data-ttu-id="7e73d-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e73d-197">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="7e73d-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e73d-198">Response</span></span>
<span data-ttu-id="7e73d-199">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-199">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="7e73d-200">После этого запроса локализация fr обновляется новым значением Баккграундколор, но в/брандинг. по умолчанию не вносятся изменения.</span><span class="sxs-lookup"><span data-stu-id="7e73d-200">Following this request, the fr localization is updated with the new value of backgroundColor, but no change is made to the default /branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="7e73d-201">Пример 4: замена фирменного стиля по умолчанию и всех локализаций</span><span class="sxs-lookup"><span data-stu-id="7e73d-201">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="7e73d-202">Если фирменная символика уже существует, при РАЗМЕЩЕНии будут заменены фирменные настройки по умолчанию и все локализации.</span><span class="sxs-lookup"><span data-stu-id="7e73d-202">If the branding already exists, PUT will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="7e73d-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e73d-203">Request</span></span>

<span data-ttu-id="7e73d-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e73d-204">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e73d-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e73d-205">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7e73d-206">C#</span><span class="sxs-lookup"><span data-stu-id="7e73d-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e73d-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e73d-207">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e73d-208">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e73d-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e73d-209">Java</span><span class="sxs-lookup"><span data-stu-id="7e73d-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e73d-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e73d-210">Response</span></span>
<span data-ttu-id="7e73d-211">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e73d-211">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="7e73d-212">В соответствии с этим запросом фирменная символика по умолчанию имеет только указанный Баккграундколор и имеет только одну локализацию с идентификатором fr, а также набор Баккграундколор.</span><span class="sxs-lookup"><span data-stu-id="7e73d-212">Following this request, the default branding has only the backgroundColor specified and has exactly one localization with the id fr, also with the backgroundColor set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
