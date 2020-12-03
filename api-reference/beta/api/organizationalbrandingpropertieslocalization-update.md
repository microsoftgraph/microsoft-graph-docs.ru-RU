---
title: Обновление локализованных организатионалбрандингпропертиес
description: Обновление свойств объекта организатионалбрандингпропертиес для определенной локализации.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 78e6ae581b1a4c0cbfd5fbff2f3814532c7491bb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49523970"
---
# <a name="update-localized-organizationalbrandingproperties"></a><span data-ttu-id="9031d-103">Обновление локализованных организатионалбрандингпропертиес</span><span class="sxs-lookup"><span data-stu-id="9031d-103">Update Localized organizationalbrandingproperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9031d-104">Обновление свойств объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) для определенной локализации.</span><span class="sxs-lookup"><span data-stu-id="9031d-104">Update the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific localization.</span></span>

## <a name="permissions"></a><span data-ttu-id="9031d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9031d-105">Permissions</span></span>

<span data-ttu-id="9031d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9031d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9031d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9031d-108">Permission type</span></span>                        | <span data-ttu-id="9031d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9031d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9031d-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9031d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9031d-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9031d-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="9031d-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9031d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9031d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9031d-113">Not supported.</span></span> |
| <span data-ttu-id="9031d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9031d-114">Application</span></span>                            | <span data-ttu-id="9031d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9031d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9031d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9031d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="9031d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9031d-117">Request headers</span></span>

| <span data-ttu-id="9031d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9031d-118">Name</span></span>       | <span data-ttu-id="9031d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9031d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9031d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9031d-120">Authorization</span></span> | <span data-ttu-id="9031d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9031d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9031d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9031d-123">Content-Type</span></span>  | <span data-ttu-id="9031d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9031d-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="9031d-126">Content — Language</span><span class="sxs-lookup"><span data-stu-id="9031d-126">Content-Language</span></span>  | <span data-ttu-id="9031d-127">Языковой стандарт.</span><span class="sxs-lookup"><span data-stu-id="9031d-127">Locale.</span></span> <span data-ttu-id="9031d-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9031d-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9031d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9031d-129">Request body</span></span>

<span data-ttu-id="9031d-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9031d-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9031d-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="9031d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9031d-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9031d-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9031d-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="9031d-133">Property</span></span>     | <span data-ttu-id="9031d-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9031d-134">Type</span></span>        | <span data-ttu-id="9031d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9031d-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9031d-136">баккграундколор</span><span class="sxs-lookup"><span data-stu-id="9031d-136">backgroundColor</span></span>|<span data-ttu-id="9031d-137">String</span><span class="sxs-lookup"><span data-stu-id="9031d-137">String</span></span>|<span data-ttu-id="9031d-138">Цвет, который будет отображаться вместо фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="9031d-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="9031d-139">Рекомендуется использовать основной цвет эмблемы баннера или цвет вашей организации.</span><span class="sxs-lookup"><span data-stu-id="9031d-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="9031d-140">Укажите в шестнадцатеричном формате (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="9031d-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="9031d-141">Изображение</span><span class="sxs-lookup"><span data-stu-id="9031d-141">backgroundImage</span></span>|<span data-ttu-id="9031d-142">Stream</span><span class="sxs-lookup"><span data-stu-id="9031d-142">Stream</span></span>|<span data-ttu-id="9031d-143">Изображение, отображаемое в качестве фона страницы входа.</span><span class="sxs-lookup"><span data-stu-id="9031d-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="9031d-144">файлы PNG или jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="9031d-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="9031d-145">Изображение меньшего размера уменьшит требования к пропускной способности и сделает загрузку страниц более производительной.</span><span class="sxs-lookup"><span data-stu-id="9031d-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="9031d-146">баннерлого</span><span class="sxs-lookup"><span data-stu-id="9031d-146">bannerLogo</span></span>|<span data-ttu-id="9031d-147">Stream</span><span class="sxs-lookup"><span data-stu-id="9031d-147">Stream</span></span>|<span data-ttu-id="9031d-148">На странице входа отображается плакатная эмблема компании.</span><span class="sxs-lookup"><span data-stu-id="9031d-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="9031d-149">файлы PNG или jpg не больше 36x245px.</span><span class="sxs-lookup"><span data-stu-id="9031d-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="9031d-150">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="9031d-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="9031d-151">сигнинпажетекст</span><span class="sxs-lookup"><span data-stu-id="9031d-151">signInPageText</span></span>|<span data-ttu-id="9031d-152">String</span><span class="sxs-lookup"><span data-stu-id="9031d-152">String</span></span>|<span data-ttu-id="9031d-153">Текст, который отображается в нижней части поля входа.</span><span class="sxs-lookup"><span data-stu-id="9031d-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="9031d-154">Вы можете использовать эту возможность для передачи дополнительных сведений, таких как номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="9031d-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="9031d-155">Этот текст должен быть Юникодом и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="9031d-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="9031d-156">скуарелого</span><span class="sxs-lookup"><span data-stu-id="9031d-156">squareLogo</span></span>|<span data-ttu-id="9031d-157">Stream</span><span class="sxs-lookup"><span data-stu-id="9031d-157">Stream</span></span>|<span data-ttu-id="9031d-158">Квадратная версия логотипа компании.</span><span class="sxs-lookup"><span data-stu-id="9031d-158">Square version of your company logo.</span></span> <span data-ttu-id="9031d-159">Эта функция отображается в режиме готовности к работе с Windows 10 (OOBE) и при включенном развертывании Windows.</span><span class="sxs-lookup"><span data-stu-id="9031d-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="9031d-160">файлы PNG или jpg не имеют размер больше 240x240px и не больше 10Kb.</span><span class="sxs-lookup"><span data-stu-id="9031d-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="9031d-161">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="9031d-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="9031d-162">усернамехинттекст</span><span class="sxs-lookup"><span data-stu-id="9031d-162">usernameHintText</span></span>|<span data-ttu-id="9031d-163">String</span><span class="sxs-lookup"><span data-stu-id="9031d-163">String</span></span>|<span data-ttu-id="9031d-164">Строка, которая отображается как подсказка в текстовом поле имя пользователя на экране входа.</span><span class="sxs-lookup"><span data-stu-id="9031d-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="9031d-165">Этот текст должен быть Юникодом без ссылок или кода и не может содержать более 64 символов.</span><span class="sxs-lookup"><span data-stu-id="9031d-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="9031d-166">id</span><span class="sxs-lookup"><span data-stu-id="9031d-166">id</span></span>|<span data-ttu-id="9031d-167">String</span><span class="sxs-lookup"><span data-stu-id="9031d-167">String</span></span>|<span data-ttu-id="9031d-168">Языковой стандарт для обновления фирменного стиля для</span><span class="sxs-lookup"><span data-stu-id="9031d-168">Locale to update branding for</span></span>|


## <a name="response"></a><span data-ttu-id="9031d-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="9031d-169">Response</span></span>

<span data-ttu-id="9031d-170">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="9031d-170">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9031d-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="9031d-171">Examples</span></span>

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a><span data-ttu-id="9031d-172">Пример 1: Настройка **баннерлого** для локализации FR с помощью метода PUT</span><span class="sxs-lookup"><span data-stu-id="9031d-172">Example 1: Setting **bannerLogo** for the fr localization using PUT</span></span>

<span data-ttu-id="9031d-173">Следующий запрос обновляет логотип баннера для локализации fr.</span><span class="sxs-lookup"><span data-stu-id="9031d-173">The following request updates the banner logo for the fr localization.</span></span> <span data-ttu-id="9031d-174">Использование метода PUT, если локализация fr не существует, возвращается значение "404 Not Found".</span><span class="sxs-lookup"><span data-stu-id="9031d-174">Using PUT, if the fr localization does not exist, "404 not found" is returned.</span></span> <span data-ttu-id="9031d-175">Если полезная нагрузка содержит свойство ID или заголовок Content-Language, и они не совпадают с идентификатором в URL-адресе, возвращается неверный запрос.</span><span class="sxs-lookup"><span data-stu-id="9031d-175">If the payload contains an id property or Content-Language header, and they don't match id in URL, a Bad Request is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="9031d-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="9031d-176">Request</span></span>

<span data-ttu-id="9031d-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9031d-177">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9031d-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="9031d-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[<span data-ttu-id="9031d-179">C#</span><span class="sxs-lookup"><span data-stu-id="9031d-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9031d-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9031d-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9031d-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9031d-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9031d-182">Java</span><span class="sxs-lookup"><span data-stu-id="9031d-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9031d-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="9031d-183">Response</span></span>

<span data-ttu-id="9031d-184">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9031d-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a><span data-ttu-id="9031d-185">Пример 2: обновление **баннерлого** для локализации FR с использованием исправления</span><span class="sxs-lookup"><span data-stu-id="9031d-185">Example 2: Update **bannerLogo** for the fr localization using PATCH</span></span>

<span data-ttu-id="9031d-186">Следующий запрос обновляет логотип баннера для локализации fr.</span><span class="sxs-lookup"><span data-stu-id="9031d-186">The following request updates the banner logo for the fr localization.</span></span>  <span data-ttu-id="9031d-187">С помощью PATCH, если указанная локализация еще не существует, она создается и в нее записывается свойство.</span><span class="sxs-lookup"><span data-stu-id="9031d-187">Using PATCH, if the specified localization does not already exist, it is created and the property is written to it.</span></span>

#### <a name="request"></a><span data-ttu-id="9031d-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="9031d-188">Request</span></span>

<span data-ttu-id="9031d-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9031d-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9031d-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="9031d-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="9031d-191">C#</span><span class="sxs-lookup"><span data-stu-id="9031d-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9031d-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9031d-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9031d-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9031d-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9031d-194">Java</span><span class="sxs-lookup"><span data-stu-id="9031d-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9031d-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="9031d-195">Response</span></span>
<span data-ttu-id="9031d-196">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9031d-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a><span data-ttu-id="9031d-197">Пример 3: замена значения по умолчанию фирменной символикой на пустую строку</span><span class="sxs-lookup"><span data-stu-id="9031d-197">Example 3: Override default branding value with a blank string</span></span>

<span data-ttu-id="9031d-198">Если значение свойства при локализации равно null, значение будет унаследовано от фирменной символики по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9031d-198">If the value of a property in a localization is null, the value will be inherited from the default branding.</span></span> <span data-ttu-id="9031d-199">Чтобы избежать этого, задайте пустую строку или строку, содержащую только пробелы в локализованной фирменной символике.</span><span class="sxs-lookup"><span data-stu-id="9031d-199">To prevent this from happening, set an empty string or string containing only whitespace in the localized branding.</span></span>

#### <a name="request"></a><span data-ttu-id="9031d-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="9031d-200">Request</span></span>

<span data-ttu-id="9031d-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9031d-201">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a><span data-ttu-id="9031d-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="9031d-202">Response</span></span>

<span data-ttu-id="9031d-203">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9031d-203">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="9031d-204">После этого запроса Усернамехинттекст для локализации будет пустым вместо того, чтобы наследовать значение из фирменной символики по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9031d-204">Following this request, usernameHintText for the fr localization will be empty instead of inheriting the value from default branding.</span></span>

### <a name="example-4-replace-french-localization-with-put"></a><span data-ttu-id="9031d-205">Пример 4: замена французской локализации на PUT</span><span class="sxs-lookup"><span data-stu-id="9031d-205">Example 4: Replace French localization with PUT</span></span>

<span data-ttu-id="9031d-206">Чтобы выполнить обновление при локализации с помощью метода PUT, мы должны добавить все свойства в тексте вместе со свойством, которое необходимо обновить при замене существующего объекта новым.</span><span class="sxs-lookup"><span data-stu-id="9031d-206">To make an update on localization using PUT, we should add all properties in body along with the property that needs to be updated as PUT replaces existing object with the new one.</span></span> <span data-ttu-id="9031d-207">Для других свойств, которые не входят в текст полезных данных PUT, будет задано значение NULL.</span><span class="sxs-lookup"><span data-stu-id="9031d-207">The other properties which are not in the payload body of PUT will be set to NULL.</span></span> <span data-ttu-id="9031d-208">В примере ниже показано, что сохраняются только свойства Баккграундколор и Сигнинпажетекст обновляются, в то время как для других задано значение null.</span><span class="sxs-lookup"><span data-stu-id="9031d-208">Here in example below, only backgroundColor property is retained and signInPageText is updated while others are set to null.</span></span>
<span data-ttu-id="9031d-209">Если указанная локализация еще не существует, укажите URL-адрес, указывающий на то, что локализация будет создана.</span><span class="sxs-lookup"><span data-stu-id="9031d-209">If the specified localization does not already exist, PUT to the URL specifying that localization creates it.</span></span>
<span data-ttu-id="9031d-210">Если полезная нагрузка содержит свойство ID или заголовок Content-Language, и они не совпадают с идентификатором в URL-адресе, то возникает ошибочный запрос.</span><span class="sxs-lookup"><span data-stu-id="9031d-210">If the payload contains an id property or a Content-Language header, and they don't match id in URL, we throw Bad request.</span></span>

#### <a name="request"></a><span data-ttu-id="9031d-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="9031d-211">Request</span></span>

<span data-ttu-id="9031d-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9031d-212">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9031d-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="9031d-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="9031d-214">C#</span><span class="sxs-lookup"><span data-stu-id="9031d-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9031d-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9031d-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9031d-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9031d-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9031d-217">Java</span><span class="sxs-lookup"><span data-stu-id="9031d-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9031d-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="9031d-218">Response</span></span>
<span data-ttu-id="9031d-219">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9031d-219">The following is an example of the response.</span></span>

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
