---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Доступ к общим элементам
localization_priority: Normal
description: Вы можете получить доступ к общим элементам DriveItem или коллекции общих элементов, используя параметр shareId или URL-адрес для совместного доступа.
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f8ca26b4e226212186f3e2716b5d4ff4c250b44f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013036"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="acaaf-103">Доступ к общим элементам DriveItem</span><span class="sxs-lookup"><span data-stu-id="acaaf-103">Accessing shared DriveItems</span></span>

<span data-ttu-id="acaaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acaaf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="acaaf-105">Вы можете получить доступ к общим элементам [DriveItem](../resources/driveitem.md) или коллекции общих элементов, используя параметр **shareId** или URL-адрес для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="acaaf-105">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="acaaf-106">Чтобы использовать URL-адрес для совместного доступа с этим API, вашему приложению необходимо [преобразовать URL-адрес в токен общего доступа](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="acaaf-106">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="acaaf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="acaaf-107">Permissions</span></span>

<span data-ttu-id="acaaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acaaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acaaf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acaaf-110">Permission type</span></span>      | <span data-ttu-id="acaaf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="acaaf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acaaf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acaaf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="acaaf-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acaaf-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="acaaf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acaaf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acaaf-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acaaf-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="acaaf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acaaf-116">Application</span></span> | <span data-ttu-id="acaaf-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acaaf-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acaaf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acaaf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="acaaf-119">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="acaaf-119">Path parameters</span></span>

| <span data-ttu-id="acaaf-120">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="acaaf-120">Parameter Name</span></span>                 | <span data-ttu-id="acaaf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="acaaf-121">Value</span></span>    | <span data-ttu-id="acaaf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="acaaf-122">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="acaaf-123">**шареидоренкодедшарингурл**</span><span class="sxs-lookup"><span data-stu-id="acaaf-123">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="acaaf-p102">Обязательный. Маркер общего доступа, возвращенный API, или правильно закодированный URL-адрес для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="acaaf-p102">Required. A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="acaaf-126">Кодирование URL-адресов для общего доступа</span><span class="sxs-lookup"><span data-stu-id="acaaf-126">Encoding sharing URLs</span></span>

<span data-ttu-id="acaaf-127">Чтобы закодировать URL-адрес для общего доступа, используйте следующую логику:</span><span class="sxs-lookup"><span data-stu-id="acaaf-127">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="acaaf-128">Для начала примените к URL-адресу кодировку base64.</span><span class="sxs-lookup"><span data-stu-id="acaaf-128">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="acaaf-129">Преобразуйте результат из кодировки base64 в [недополненный формат base64url](https://en.wikipedia.org/wiki/Base64), удалив символы `=` в конце значения и заменив `/` символом `_`, а `+` — символом `-`.)</span><span class="sxs-lookup"><span data-stu-id="acaaf-129">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="acaaf-130">Добавьте `u!` в начало строки.</span><span class="sxs-lookup"><span data-stu-id="acaaf-130">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="acaaf-131">Пример кодирования URL-адреса на языке C#:</span><span class="sxs-lookup"><span data-stu-id="acaaf-131">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="acaaf-132">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acaaf-132">Optional request headers</span></span>

| <span data-ttu-id="acaaf-133">Имя</span><span class="sxs-lookup"><span data-stu-id="acaaf-133">Name</span></span>       | <span data-ttu-id="acaaf-134">Тип</span><span class="sxs-lookup"><span data-stu-id="acaaf-134">Type</span></span>   | <span data-ttu-id="acaaf-135">Описание</span><span class="sxs-lookup"><span data-stu-id="acaaf-135">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="acaaf-136">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="acaaf-136">**Prefer**</span></span> | <span data-ttu-id="acaaf-137">string</span><span class="sxs-lookup"><span data-stu-id="acaaf-137">string</span></span> | <span data-ttu-id="acaaf-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="acaaf-138">Optional.</span></span> <span data-ttu-id="acaaf-139">Установите одно из значений, приведенных `prefer` ниже.</span><span class="sxs-lookup"><span data-stu-id="acaaf-139">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="acaaf-140">Предпочтительные значения заголовков</span><span class="sxs-lookup"><span data-stu-id="acaaf-140">Prefer header values</span></span>

| <span data-ttu-id="acaaf-141">Имя</span><span class="sxs-lookup"><span data-stu-id="acaaf-141">Name</span></span>                          | <span data-ttu-id="acaaf-142">Описание</span><span class="sxs-lookup"><span data-stu-id="acaaf-142">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="acaaf-143">редимшаринглинк</span><span class="sxs-lookup"><span data-stu-id="acaaf-143">redeemSharingLink</span></span>             | <span data-ttu-id="acaaf-144">Если **шареидоренкодедшарингурл** представляет собой ссылку для совместного доступа, предоставьте вызывающему методу долговременный доступ к элементу</span><span class="sxs-lookup"><span data-stu-id="acaaf-144">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="acaaf-145">редимшаринглинкифнецессари</span><span class="sxs-lookup"><span data-stu-id="acaaf-145">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="acaaf-146">То же, что и Редимшаринглинк, но доступ гарантированно предоставляется только в течение этого запроса.</span><span class="sxs-lookup"><span data-stu-id="acaaf-146">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="acaaf-147">Редимшаринглинк должен считаться эквивалентным участнику, который перемещается в ссылку для совместного доступа, в браузере (принимается жестом общего доступа), тогда как Редимшаринглинкифнецессари предназначена для сценариев, в которых намерением является простой просмотр метаданных ссылки.</span><span class="sxs-lookup"><span data-stu-id="acaaf-147">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="acaaf-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="acaaf-148">Response</span></span>

<span data-ttu-id="acaaf-149">При успешном выполнении этот метод возвращает код отклика `200 OK` и ресурс [sharedDriveItem](../resources/shareddriveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="acaaf-149">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acaaf-150">Пример</span><span class="sxs-lookup"><span data-stu-id="acaaf-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="acaaf-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="acaaf-151">Request</span></span>

<span data-ttu-id="acaaf-152">Вот пример запроса для получения общего элемента:</span><span class="sxs-lookup"><span data-stu-id="acaaf-152">Here is an example of the request to retrieve a shared item:</span></span>


# <a name="http"></a>[<span data-ttu-id="acaaf-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="acaaf-153">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-root" } -->

```msgraph-interactive
GET /shares/{shareIdOrEncodedSharingUrl}
```
# <a name="c"></a>[<span data-ttu-id="acaaf-154">C#</span><span class="sxs-lookup"><span data-stu-id="acaaf-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acaaf-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acaaf-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acaaf-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acaaf-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acaaf-157">Java</span><span class="sxs-lookup"><span data-stu-id="acaaf-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="acaaf-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="acaaf-158">Response</span></span>

<span data-ttu-id="acaaf-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="acaaf-159">Here is an example of the response.</span></span>

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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="acaaf-160">Прямой доступ к общему элементу</span><span class="sxs-lookup"><span data-stu-id="acaaf-160">Access the shared item directly</span></span>

<span data-ttu-id="acaaf-p104">Так как элемент [**SharedDriveItem**](../resources/shareddriveitem.md) содержит полезную информацию, большинство приложений будут стремиться получить прямой доступ к общему элементу [DriveItem](../resources/driveitem.md). Ресурс **SharedDriveItem** включает связи **корня** и **элементов**, которые могут получать доступ к содержимому в области общего элемента.</span><span class="sxs-lookup"><span data-stu-id="acaaf-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="acaaf-163">Пример (один файл)</span><span class="sxs-lookup"><span data-stu-id="acaaf-163">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="acaaf-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="acaaf-164">Request</span></span>

<span data-ttu-id="acaaf-165">При запросе связи **driveItem** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="acaaf-165">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="acaaf-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="acaaf-166">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```msgraph-interactive
GET /shares/{shareIdOrUrl}/driveItem
```
# <a name="c"></a>[<span data-ttu-id="acaaf-167">C#</span><span class="sxs-lookup"><span data-stu-id="acaaf-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acaaf-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acaaf-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acaaf-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acaaf-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acaaf-170">Java</span><span class="sxs-lookup"><span data-stu-id="acaaf-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-driveitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="acaaf-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="acaaf-171">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="acaaf-172">Пример (общая папка)</span><span class="sxs-lookup"><span data-stu-id="acaaf-172">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="acaaf-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="acaaf-173">Request</span></span>

<span data-ttu-id="acaaf-174">При запросе связи **driveItem** и расширении коллекции **children** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ, а также файлы, содержащиеся в общей папке.</span><span class="sxs-lookup"><span data-stu-id="acaaf-174">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>


# <a name="http"></a>[<span data-ttu-id="acaaf-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="acaaf-175">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```msgraph-interactive
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```
# <a name="c"></a>[<span data-ttu-id="acaaf-176">C#</span><span class="sxs-lookup"><span data-stu-id="acaaf-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shared-driveitem-expand-children-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acaaf-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acaaf-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shared-driveitem-expand-children-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acaaf-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acaaf-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shared-driveitem-expand-children-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acaaf-179">Java</span><span class="sxs-lookup"><span data-stu-id="acaaf-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-shared-driveitem-expand-children-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="acaaf-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="acaaf-180">Response</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="acaaf-181">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="acaaf-181">Error Responses</span></span>

<span data-ttu-id="acaaf-182">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="acaaf-182">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="acaaf-183">Замечания</span><span class="sxs-lookup"><span data-stu-id="acaaf-183">Remarks</span></span>

* <span data-ttu-id="acaaf-184">В случае OneDrive для бизнеса и SharePoint API общих ресурсов всегда требует аутентификации. С его помощью невозможно обращаться к содержимому, доступ к которому предоставлен анонимно, без контекста пользователя.</span><span class="sxs-lookup"><span data-stu-id="acaaf-184">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link",
  "suppressions": [
  ]
} -->

