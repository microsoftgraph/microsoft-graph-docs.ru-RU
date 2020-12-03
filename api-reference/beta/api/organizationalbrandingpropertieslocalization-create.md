---
title: Создание локализованных Организатионалбрандингпропертиес
description: Создание фирменной символики Организации для определенного языкового стандарта.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c293085887eb0e8c2d49c4e01c567dbeea32699
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524432"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="a2665-103">Создание локализованных Организатионалбрандингпропертиес</span><span class="sxs-lookup"><span data-stu-id="a2665-103">Create localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2665-104">Создание объекта [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) для определенного языкового стандарта.</span><span class="sxs-lookup"><span data-stu-id="a2665-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2665-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2665-105">Permissions</span></span>

<span data-ttu-id="a2665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2665-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2665-108">Permission type</span></span>                        | <span data-ttu-id="a2665-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2665-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a2665-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2665-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2665-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2665-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="a2665-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2665-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2665-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2665-113">Not supported.</span></span> |
| <span data-ttu-id="a2665-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2665-114">Application</span></span>                            | <span data-ttu-id="a2665-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2665-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2665-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2665-116">HTTP request</span></span>

<span data-ttu-id="a2665-117">Разместите в фирменной символике/локализации, чтобы создать новую локализацию.</span><span class="sxs-lookup"><span data-stu-id="a2665-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="a2665-118">Идентификатор, указанный в теле, — это языковой стандарт локализации.</span><span class="sxs-lookup"><span data-stu-id="a2665-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="a2665-119">Если идентификатор не указан, то в качестве идентификатора используется значение заголовка Content-Language, если оно указано. Если заголовок ID и Content-Language не указаны, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="a2665-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2665-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2665-120">Optional query parameters</span></span>

<span data-ttu-id="a2665-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a2665-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a2665-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a2665-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2665-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2665-123">Request headers</span></span>

| <span data-ttu-id="a2665-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a2665-124">Name</span></span>      |<span data-ttu-id="a2665-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a2665-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a2665-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2665-126">Authorization</span></span> | <span data-ttu-id="a2665-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2665-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a2665-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2665-129">Content-Type</span></span>  | <span data-ttu-id="a2665-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2665-p105">application/json. Required.</span></span>  |
| <span data-ttu-id="a2665-132">Content — Language</span><span class="sxs-lookup"><span data-stu-id="a2665-132">Content-Language</span></span>  | <span data-ttu-id="a2665-133">Языковой стандарт.</span><span class="sxs-lookup"><span data-stu-id="a2665-133">Locale.</span></span> <span data-ttu-id="a2665-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a2665-134">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2665-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2665-135">Request body</span></span>

<span data-ttu-id="a2665-136">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a2665-136">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a2665-137">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a2665-137">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a2665-138">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a2665-138">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a2665-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2665-139">Property</span></span>     | <span data-ttu-id="a2665-140">Тип</span><span class="sxs-lookup"><span data-stu-id="a2665-140">Type</span></span>        | <span data-ttu-id="a2665-141">Описание</span><span class="sxs-lookup"><span data-stu-id="a2665-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2665-142">баккграундколор</span><span class="sxs-lookup"><span data-stu-id="a2665-142">backgroundColor</span></span>|<span data-ttu-id="a2665-143">String</span><span class="sxs-lookup"><span data-stu-id="a2665-143">String</span></span>|<span data-ttu-id="a2665-144">Цвет, который будет отображаться вместо фонового изображения в подключениях с низкой пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="a2665-144">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="a2665-145">Рекомендуется использовать основной цвет эмблемы баннера или цвет вашей организации.</span><span class="sxs-lookup"><span data-stu-id="a2665-145">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="a2665-146">Укажите в шестнадцатеричном формате (например, белый #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="a2665-146">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="a2665-147">Изображение</span><span class="sxs-lookup"><span data-stu-id="a2665-147">backgroundImage</span></span>|<span data-ttu-id="a2665-148">Stream</span><span class="sxs-lookup"><span data-stu-id="a2665-148">Stream</span></span>|<span data-ttu-id="a2665-149">Изображение, отображаемое в качестве фона страницы входа.</span><span class="sxs-lookup"><span data-stu-id="a2665-149">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="a2665-150">файлы PNG или jpg не больше 1920x1080 и меньше 300kb.</span><span class="sxs-lookup"><span data-stu-id="a2665-150">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="a2665-151">Изображение меньшего размера уменьшит требования к пропускной способности и сделает загрузку страниц более производительной.</span><span class="sxs-lookup"><span data-stu-id="a2665-151">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="a2665-152">баннерлого</span><span class="sxs-lookup"><span data-stu-id="a2665-152">bannerLogo</span></span>|<span data-ttu-id="a2665-153">Stream</span><span class="sxs-lookup"><span data-stu-id="a2665-153">Stream</span></span>|<span data-ttu-id="a2665-154">На странице входа отображается плакатная эмблема компании.</span><span class="sxs-lookup"><span data-stu-id="a2665-154">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="a2665-155">файлы PNG или jpg не больше 36x245px.</span><span class="sxs-lookup"><span data-stu-id="a2665-155">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="a2665-156">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="a2665-156">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="a2665-157">сигнинпажетекст</span><span class="sxs-lookup"><span data-stu-id="a2665-157">signInPageText</span></span>|<span data-ttu-id="a2665-158">String</span><span class="sxs-lookup"><span data-stu-id="a2665-158">String</span></span>|<span data-ttu-id="a2665-159">Текст, который отображается в нижней части поля входа.</span><span class="sxs-lookup"><span data-stu-id="a2665-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="a2665-160">Вы можете использовать эту возможность для передачи дополнительных сведений, таких как номер телефона в службу поддержки или юридический отчет.</span><span class="sxs-lookup"><span data-stu-id="a2665-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="a2665-161">Этот текст должен быть Юникодом и не превышать 1024 символов.</span><span class="sxs-lookup"><span data-stu-id="a2665-161">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="a2665-162">скуарелого</span><span class="sxs-lookup"><span data-stu-id="a2665-162">squareLogo</span></span>|<span data-ttu-id="a2665-163">Stream</span><span class="sxs-lookup"><span data-stu-id="a2665-163">Stream</span></span>|<span data-ttu-id="a2665-164">Квадратная версия логотипа компании.</span><span class="sxs-lookup"><span data-stu-id="a2665-164">Square version of your company logo.</span></span> <span data-ttu-id="a2665-165">Эта функция отображается в режиме готовности к работе с Windows 10 (OOBE) и при включенном развертывании Windows.</span><span class="sxs-lookup"><span data-stu-id="a2665-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="a2665-166">файлы PNG или jpg не имеют размер больше 240x240px и не больше 10Kb.</span><span class="sxs-lookup"><span data-stu-id="a2665-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="a2665-167">Мы рекомендуем использовать прозрачное изображение без заполнения вокруг логотипа.</span><span class="sxs-lookup"><span data-stu-id="a2665-167">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="a2665-168">усернамехинттекст</span><span class="sxs-lookup"><span data-stu-id="a2665-168">usernameHintText</span></span>|<span data-ttu-id="a2665-169">String</span><span class="sxs-lookup"><span data-stu-id="a2665-169">String</span></span>|<span data-ttu-id="a2665-170">Строка, которая отображается как подсказка в текстовом поле имя пользователя на экране входа.</span><span class="sxs-lookup"><span data-stu-id="a2665-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="a2665-171">Этот текст должен быть Юникодом без ссылок или кода и не может содержать более 64 символов.</span><span class="sxs-lookup"><span data-stu-id="a2665-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="a2665-172">id</span><span class="sxs-lookup"><span data-stu-id="a2665-172">id</span></span>|<span data-ttu-id="a2665-173">String</span><span class="sxs-lookup"><span data-stu-id="a2665-173">String</span></span>|<span data-ttu-id="a2665-174">Языковой стандарт для создания фирменной символики для</span><span class="sxs-lookup"><span data-stu-id="a2665-174">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="a2665-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2665-175">Response</span></span>

<span data-ttu-id="a2665-176">В случае успешного выполнения этот метод возвращает `201 CREATED` код отклика и созданный объект [организатионалбрандингпропертиес](../resources/organizationalbrandingproperties.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2665-176">If successful, this method returns a `201 CREATED` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2665-177">Примеры</span><span class="sxs-lookup"><span data-stu-id="a2665-177">Examples</span></span>

<span data-ttu-id="a2665-178">В приведенном ниже примере создается локализация фирменного стиля для французского языка (fr).</span><span class="sxs-lookup"><span data-stu-id="a2665-178">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="a2665-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2665-179">Request</span></span>

<span data-ttu-id="a2665-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2665-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a2665-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2665-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="a2665-182">C#</span><span class="sxs-lookup"><span data-stu-id="a2665-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2665-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2665-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2665-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2665-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a2665-185">Java</span><span class="sxs-lookup"><span data-stu-id="a2665-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a2665-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2665-186">Response</span></span>

<span data-ttu-id="a2665-187">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a2665-187">The following is an example of the response.</span></span>

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
<span data-ttu-id="a2665-188">**Медиаедитлинк** указывает, где записывается локализованный носитель.</span><span class="sxs-lookup"><span data-stu-id="a2665-188">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="a2665-189">Медиареадлинк имеет значение null, так как для локализации не задан носитель.</span><span class="sxs-lookup"><span data-stu-id="a2665-189">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
