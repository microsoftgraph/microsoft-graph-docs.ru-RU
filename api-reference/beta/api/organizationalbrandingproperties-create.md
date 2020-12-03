---
title: Создание Организатионалбрандингпропертиес
description: Создание фирменной символики Организации.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adf9a1e6b3f0bb01cbe028b27822b139d736d42e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524619"
---
# <a name="create-organizationalbrandingproperties"></a><span data-ttu-id="79a45-103">Создание Организатионалбрандингпропертиес</span><span class="sxs-lookup"><span data-stu-id="79a45-103">Create organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79a45-104">Создание объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="79a45-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="79a45-105">При этом создается фирменная символика по умолчанию и, при необходимости, локализованная фирменная символика.</span><span class="sxs-lookup"><span data-stu-id="79a45-105">This creates the default branding and optionally a localized branding at the same time.</span></span> <span data-ttu-id="79a45-106">Фирменная символика по умолчанию загружается, когда локализованный набор фирменного стиля не настроен для языка браузера пользователя.</span><span class="sxs-lookup"><span data-stu-id="79a45-106">The default branding is loaded when a localized branding set isn't configured for the user's browser language.</span></span>

## <a name="permissions"></a><span data-ttu-id="79a45-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79a45-107">Permissions</span></span>

<span data-ttu-id="79a45-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79a45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79a45-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79a45-110">Permission type</span></span>                        | <span data-ttu-id="79a45-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79a45-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79a45-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79a45-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="79a45-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79a45-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="79a45-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79a45-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79a45-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79a45-115">Not supported.</span></span> |
| <span data-ttu-id="79a45-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79a45-116">Application</span></span>                            | <span data-ttu-id="79a45-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79a45-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="79a45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79a45-118">HTTP request</span></span>

<span data-ttu-id="79a45-119">Фирменная символика создается для Организации, если она еще не существует, с помощью функции "вставить" или "исправить".</span><span class="sxs-lookup"><span data-stu-id="79a45-119">A branding is created for an organization, if one does not already exist, using PUT or PATCH.</span></span>

<span data-ttu-id="79a45-120">Если фирменная символика уже настроена, при РАЗМЕЩЕНии будут перезаписаны все существующие значения независимо от того, что находится в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="79a45-120">If branding is already configured, PUT will overwrite all existing values regardless of what's in the request body.</span></span> <span data-ttu-id="79a45-121">PATCH будет оверите только значения, включенные в текст запроса, оставляя значения, не включенные в неизмененное.</span><span class="sxs-lookup"><span data-stu-id="79a45-121">PATCH will only overite the values that are included in the request body, leaving the values not included unchanged.</span></span>

<span data-ttu-id="79a45-122">Свойство **ID** игнорируется на странице PUT/patch для одноэлементного экземпляра/брандинг.</span><span class="sxs-lookup"><span data-stu-id="79a45-122">The **id** property is ignored on PUT/PATCH to the /branding singleton.</span></span> <span data-ttu-id="79a45-123">Если язык содержимого не указан, создается фирменная символика по умолчанию, соответствующая **идентификатору** `und` .</span><span class="sxs-lookup"><span data-stu-id="79a45-123">If Content-Language is not specified, the default branding is created, which corresponds to an **id** of `und`.</span></span> <span data-ttu-id="79a45-124">Если указан язык содержимого, для этого языкового стандарта создается фирменная символика.</span><span class="sxs-lookup"><span data-stu-id="79a45-124">If Content-Language is specified, branding is created for that locale.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79a45-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79a45-125">Optional query parameters</span></span>

<span data-ttu-id="79a45-126">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="79a45-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="79a45-127">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="79a45-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="79a45-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79a45-128">Request headers</span></span>

| <span data-ttu-id="79a45-129">Имя</span><span class="sxs-lookup"><span data-stu-id="79a45-129">Name</span></span>      |<span data-ttu-id="79a45-130">Описание</span><span class="sxs-lookup"><span data-stu-id="79a45-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79a45-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79a45-131">Authorization</span></span> | <span data-ttu-id="79a45-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79a45-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79a45-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79a45-134">Content-Type</span></span>  | <span data-ttu-id="79a45-p107">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79a45-p107">application/json. Required.</span></span>  |
| <span data-ttu-id="79a45-137">Content — Language</span><span class="sxs-lookup"><span data-stu-id="79a45-137">Content-Language</span></span>  | <span data-ttu-id="79a45-138">Языковой стандарт.</span><span class="sxs-lookup"><span data-stu-id="79a45-138">Locale.</span></span> <span data-ttu-id="79a45-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="79a45-139">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79a45-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79a45-140">Request body</span></span>

| <span data-ttu-id="79a45-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="79a45-141">Property</span></span>     | <span data-ttu-id="79a45-142">Тип</span><span class="sxs-lookup"><span data-stu-id="79a45-142">Type</span></span>        | <span data-ttu-id="79a45-143">Описание</span><span class="sxs-lookup"><span data-stu-id="79a45-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79a45-144">баккграундколор</span><span class="sxs-lookup"><span data-stu-id="79a45-144">backgroundColor</span></span>|<span data-ttu-id="79a45-145">String</span><span class="sxs-lookup"><span data-stu-id="79a45-145">String</span></span>|<span data-ttu-id="79a45-146">Цвет, который будет отображаться вместо фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="79a45-146">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="79a45-147">Рекомендуется использовать основной цвет эмблемы баннера или цвет вашей организации.</span><span class="sxs-lookup"><span data-stu-id="79a45-147">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="79a45-148">Укажите в шестнадцатеричном формате (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="79a45-148">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="79a45-149">Изображение</span><span class="sxs-lookup"><span data-stu-id="79a45-149">backgroundImage</span></span>|<span data-ttu-id="79a45-150">Stream</span><span class="sxs-lookup"><span data-stu-id="79a45-150">Stream</span></span>|<span data-ttu-id="79a45-151">Изображение, отображаемое в качестве фона страницы входа.</span><span class="sxs-lookup"><span data-stu-id="79a45-151">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="79a45-152">файлы PNG или jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="79a45-152">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="79a45-153">Изображение меньшего размера уменьшит требования к пропускной способности и сделает загрузку страниц более производительной.</span><span class="sxs-lookup"><span data-stu-id="79a45-153">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="79a45-154">баннерлого</span><span class="sxs-lookup"><span data-stu-id="79a45-154">bannerLogo</span></span>|<span data-ttu-id="79a45-155">Stream</span><span class="sxs-lookup"><span data-stu-id="79a45-155">Stream</span></span>|<span data-ttu-id="79a45-156">На странице входа отображается плакатная эмблема компании.</span><span class="sxs-lookup"><span data-stu-id="79a45-156">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="79a45-157">файлы PNG или jpg не больше 36x245px.</span><span class="sxs-lookup"><span data-stu-id="79a45-157">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="79a45-158">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="79a45-158">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="79a45-159">сигнинпажетекст</span><span class="sxs-lookup"><span data-stu-id="79a45-159">signInPageText</span></span>|<span data-ttu-id="79a45-160">String</span><span class="sxs-lookup"><span data-stu-id="79a45-160">String</span></span>|<span data-ttu-id="79a45-161">Текст, который отображается в нижней части поля входа.</span><span class="sxs-lookup"><span data-stu-id="79a45-161">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="79a45-162">Вы можете использовать эту возможность для передачи дополнительных сведений, таких как номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="79a45-162">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="79a45-163">Этот текст должен быть Юникодом и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="79a45-163">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="79a45-164">скуарелого</span><span class="sxs-lookup"><span data-stu-id="79a45-164">squareLogo</span></span>|<span data-ttu-id="79a45-165">Stream</span><span class="sxs-lookup"><span data-stu-id="79a45-165">Stream</span></span>|<span data-ttu-id="79a45-166">Квадратная версия логотипа компании.</span><span class="sxs-lookup"><span data-stu-id="79a45-166">Square version of your company logo.</span></span> <span data-ttu-id="79a45-167">Эта функция отображается в режиме готовности к работе с Windows 10 (OOBE) и при включенном развертывании Windows.</span><span class="sxs-lookup"><span data-stu-id="79a45-167">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="79a45-168">файлы PNG или jpg не имеют размер больше 240x240px и не больше 10Kb.</span><span class="sxs-lookup"><span data-stu-id="79a45-168">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="79a45-169">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="79a45-169">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="79a45-170">усернамехинттекст</span><span class="sxs-lookup"><span data-stu-id="79a45-170">usernameHintText</span></span>|<span data-ttu-id="79a45-171">String</span><span class="sxs-lookup"><span data-stu-id="79a45-171">String</span></span>|<span data-ttu-id="79a45-172">Строка, которая отображается как подсказка в текстовом поле имя пользователя на экране входа.</span><span class="sxs-lookup"><span data-stu-id="79a45-172">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="79a45-173">Этот текст должен быть Юникодом без ссылок или кода и не может содержать более 64 символов.</span><span class="sxs-lookup"><span data-stu-id="79a45-173">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="79a45-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="79a45-174">Response</span></span>

<span data-ttu-id="79a45-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и созданный объект [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79a45-175">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79a45-176">Примеры</span><span class="sxs-lookup"><span data-stu-id="79a45-176">Examples</span></span>

<span data-ttu-id="79a45-177">В следующем примере показано, как создать фирменную символику и локализацию по умолчанию для en/US.</span><span class="sxs-lookup"><span data-stu-id="79a45-177">The following example creates default branding and localization for en-US.</span></span>

### <a name="request"></a><span data-ttu-id="79a45-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="79a45-178">Request</span></span>

<span data-ttu-id="79a45-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79a45-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79a45-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="79a45-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
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
# <a name="c"></a>[<span data-ttu-id="79a45-181">C#</span><span class="sxs-lookup"><span data-stu-id="79a45-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79a45-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79a45-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79a45-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79a45-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79a45-184">Java</span><span class="sxs-lookup"><span data-stu-id="79a45-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79a45-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="79a45-185">Response</span></span>

<span data-ttu-id="79a45-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79a45-186">The following is an example of the response.</span></span>

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

<span data-ttu-id="79a45-187">В этом случае задается объект фирменной символики по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="79a45-187">In this case, the default branding object is set.</span></span> <span data-ttu-id="79a45-188">Локализованная фирменная символика для en-US также устанавливается из-за того, что в заголовке используется язык контента, даже если в ответе не возвращается набор фирменной символики en-US.</span><span class="sxs-lookup"><span data-stu-id="79a45-188">Localized branding for en-US is also set due to the Content-Language in the header, even though the en-US branding set is not returned in the response.</span></span> <span data-ttu-id="79a45-189">Обратите внимание на то, что язык контента в запросе является необязательным, и если он отсутствует, будет задана фирменная символика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="79a45-189">Note that Content-Language in the request is optional, and if not present, will only set default branding.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
