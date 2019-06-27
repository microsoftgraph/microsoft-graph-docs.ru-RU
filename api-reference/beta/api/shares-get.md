---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Доступ к общим элементам
localization_priority: Normal
ms.openlocfilehash: 5988ca36f140c8b8ef48d5e2f7ab5f9c276a3847
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263758"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="00ae5-102">Доступ к общим элементам DriveItem</span><span class="sxs-lookup"><span data-stu-id="00ae5-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="00ae5-103">Вы можете получить доступ к общим элементам [DriveItem](../resources/driveitem.md) или коллекции общих элементов, используя параметр **shareId** или URL-адрес для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="00ae5-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="00ae5-104">Чтобы использовать URL-адрес для совместного доступа с этим API, вашему приложению необходимо [преобразовать URL-адрес в токен общего доступа](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="00ae5-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="00ae5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00ae5-105">Permissions</span></span>

<span data-ttu-id="00ae5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00ae5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ae5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00ae5-108">Permission type</span></span>      | <span data-ttu-id="00ae5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00ae5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00ae5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00ae5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00ae5-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ae5-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="00ae5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00ae5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00ae5-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ae5-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="00ae5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00ae5-114">Application</span></span> | <span data-ttu-id="00ae5-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ae5-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00ae5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00ae5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="00ae5-117">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="00ae5-117">Path parameters</span></span>

| <span data-ttu-id="00ae5-118">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="00ae5-118">Parameter Name</span></span>                 | <span data-ttu-id="00ae5-119">Значение</span><span class="sxs-lookup"><span data-stu-id="00ae5-119">Value</span></span>    | <span data-ttu-id="00ae5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="00ae5-120">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="00ae5-121">**Шареидоренкодедшарингурл**</span><span class="sxs-lookup"><span data-stu-id="00ae5-121">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="00ae5-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00ae5-122">Required.</span></span> <span data-ttu-id="00ae5-123">Маркер общего доступа, возвращенный API, или правильно закодированный URL-адрес для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="00ae5-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="00ae5-124">Кодирование URL-адресов для общего доступа</span><span class="sxs-lookup"><span data-stu-id="00ae5-124">Encoding sharing URLs</span></span>

<span data-ttu-id="00ae5-125">Чтобы закодировать URL-адрес для общего доступа, используйте следующую логику:</span><span class="sxs-lookup"><span data-stu-id="00ae5-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="00ae5-126">Для начала примените к URL-адресу кодировку base64.</span><span class="sxs-lookup"><span data-stu-id="00ae5-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="00ae5-127">Преобразуйте результат из кодировки base64 в [недополненный формат base64url](https://en.wikipedia.org/wiki/Base64), удалив символы `=` в конце значения и заменив `/` символом `_`, а `+` — символом `-`.)</span><span class="sxs-lookup"><span data-stu-id="00ae5-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="00ae5-128">Добавьте `u!` в начало строки.</span><span class="sxs-lookup"><span data-stu-id="00ae5-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="00ae5-129">Пример кодирования URL-адреса на C#:</span><span class="sxs-lookup"><span data-stu-id="00ae5-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="00ae5-130">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00ae5-130">Optional request headers</span></span>

| <span data-ttu-id="00ae5-131">Имя</span><span class="sxs-lookup"><span data-stu-id="00ae5-131">Name</span></span>       | <span data-ttu-id="00ae5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="00ae5-132">Type</span></span>   | <span data-ttu-id="00ae5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="00ae5-133">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="00ae5-134">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="00ae5-134">**Prefer**</span></span> | <span data-ttu-id="00ae5-135">string</span><span class="sxs-lookup"><span data-stu-id="00ae5-135">string</span></span> | <span data-ttu-id="00ae5-136">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="00ae5-136">Optional.</span></span> <span data-ttu-id="00ae5-137">Установите одно из значений, `prefer` приведенных ниже.</span><span class="sxs-lookup"><span data-stu-id="00ae5-137">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="00ae5-138">Предпочтительные значения заголовков</span><span class="sxs-lookup"><span data-stu-id="00ae5-138">Prefer header values</span></span>

| <span data-ttu-id="00ae5-139">Имя</span><span class="sxs-lookup"><span data-stu-id="00ae5-139">Name</span></span>                          | <span data-ttu-id="00ae5-140">Описание</span><span class="sxs-lookup"><span data-stu-id="00ae5-140">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="00ae5-141">Редимшаринглинк</span><span class="sxs-lookup"><span data-stu-id="00ae5-141">redeemSharingLink</span></span>             | <span data-ttu-id="00ae5-142">Если **шареидоренкодедшарингурл** представляет собой ссылку для совместного доступа, предоставьте вызывающему методу долговременный доступ к элементу</span><span class="sxs-lookup"><span data-stu-id="00ae5-142">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="00ae5-143">Редимшаринглинкифнецессари</span><span class="sxs-lookup"><span data-stu-id="00ae5-143">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="00ae5-144">То же, что и Редимшаринглинк, но доступ гарантированно предоставляется только в течение этого запроса.</span><span class="sxs-lookup"><span data-stu-id="00ae5-144">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="00ae5-145">Редимшаринглинк должен считаться эквивалентным участнику, который перемещается в ссылку для совместного доступа, в браузере (принимается жестом общего доступа), тогда как Редимшаринглинкифнецессари предназначено для сценариев, в которых намерением является просто взглянуть на ссылку метаданных.</span><span class="sxs-lookup"><span data-stu-id="00ae5-145">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="00ae5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="00ae5-146">Response</span></span>

<span data-ttu-id="00ae5-147">При успешном выполнении этот метод возвращает код отклика `200 OK` и ресурс [sharedDriveItem](../resources/shareddriveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00ae5-147">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00ae5-148">Пример</span><span class="sxs-lookup"><span data-stu-id="00ae5-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="00ae5-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="00ae5-149">Request</span></span>

<span data-ttu-id="00ae5-150">Вот пример запроса для получения общего элемента:</span><span class="sxs-lookup"><span data-stu-id="00ae5-150">Here is an example of the request to retrieve a shared item:</span></span>

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a><span data-ttu-id="00ae5-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="00ae5-151">Response</span></span>

<span data-ttu-id="00ae5-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00ae5-152">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="00ae5-153">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="00ae5-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="00ae5-154">C#</span><span class="sxs-lookup"><span data-stu-id="00ae5-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-root-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00ae5-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="00ae5-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-root-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="00ae5-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="00ae5-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-root-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="00ae5-157">Прямой доступ к общему элементу</span><span class="sxs-lookup"><span data-stu-id="00ae5-157">Access the shared item directly</span></span>

<span data-ttu-id="00ae5-p104">Так как элемент [**SharedDriveItem**](../resources/shareddriveitem.md) содержит полезную информацию, большинство приложений будут стремиться получить прямой доступ к общему элементу [DriveItem](../resources/driveitem.md). Ресурс **SharedDriveItem** включает связи **корня** и **элементов**, которые могут получать доступ к содержимому в области общего элемента.</span><span class="sxs-lookup"><span data-stu-id="00ae5-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="00ae5-160">Пример (один файл)</span><span class="sxs-lookup"><span data-stu-id="00ae5-160">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="00ae5-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="00ae5-161">Request</span></span>

<span data-ttu-id="00ae5-162">При запросе связи **driveItem** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="00ae5-162">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a><span data-ttu-id="00ae5-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="00ae5-163">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="00ae5-164">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="00ae5-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="00ae5-165">C#</span><span class="sxs-lookup"><span data-stu-id="00ae5-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00ae5-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="00ae5-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="00ae5-167">Цель — C</span><span class="sxs-lookup"><span data-stu-id="00ae5-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-shared-folder"></a><span data-ttu-id="00ae5-168">Пример (общая папка)</span><span class="sxs-lookup"><span data-stu-id="00ae5-168">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="00ae5-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="00ae5-169">Request</span></span>

<span data-ttu-id="00ae5-170">При запросе связи **driveItem** и расширении коллекции **children** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ, а также файлы, содержащиеся в общей папке.</span><span class="sxs-lookup"><span data-stu-id="00ae5-170">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a><span data-ttu-id="00ae5-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="00ae5-171">Response</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="00ae5-172">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="00ae5-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="00ae5-173">C#</span><span class="sxs-lookup"><span data-stu-id="00ae5-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00ae5-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="00ae5-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="00ae5-175">Цель — C</span><span class="sxs-lookup"><span data-stu-id="00ae5-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-shared-driveitem-expand-children-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="00ae5-176">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="00ae5-176">Error Responses</span></span>

<span data-ttu-id="00ae5-177">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="00ae5-177">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="00ae5-178">Замечания</span><span class="sxs-lookup"><span data-stu-id="00ae5-178">Remarks</span></span>

* <span data-ttu-id="00ae5-179">В случае OneDrive для бизнеса и SharePoint API общих ресурсов всегда требует аутентификации. С его помощью невозможно обращаться к содержимому, доступ к которому предоставлен анонимно, без контекста пользователя.</span><span class="sxs-lookup"><span data-stu-id="00ae5-179">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link",
  "suppressions": [
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shares-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
