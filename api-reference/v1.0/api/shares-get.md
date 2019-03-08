---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Доступ к общим элементам
localization_priority: Normal
ms.openlocfilehash: 1f172060a8b30996ff09b3ca93390da503db9fea
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480658"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="7cf93-102">Доступ к общим элементам DriveItem</span><span class="sxs-lookup"><span data-stu-id="7cf93-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="7cf93-103">Вы можете получить доступ к общим элементам [DriveItem](../resources/driveitem.md) или коллекции общих элементов, используя параметр **shareId** или URL-адрес для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="7cf93-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="7cf93-104">Чтобы использовать URL-адрес для совместного доступа с этим API, вашему приложению необходимо [преобразовать URL-адрес в токен общего доступа](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="7cf93-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="7cf93-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cf93-105">Permissions</span></span>

<span data-ttu-id="7cf93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cf93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cf93-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cf93-108">Permission type</span></span>      | <span data-ttu-id="7cf93-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cf93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cf93-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cf93-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7cf93-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf93-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7cf93-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cf93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cf93-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf93-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7cf93-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7cf93-114">Application</span></span> | <span data-ttu-id="7cf93-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf93-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cf93-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cf93-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="7cf93-117">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="7cf93-117">Path parameters</span></span>

| <span data-ttu-id="7cf93-118">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="7cf93-118">Parameter Name</span></span>                 | <span data-ttu-id="7cf93-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7cf93-119">Value</span></span>    | <span data-ttu-id="7cf93-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf93-120">Description</span></span>                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="7cf93-121">**Шареидоренкодедшарингурл**</span><span class="sxs-lookup"><span data-stu-id="7cf93-121">**shareIdOrEncodedSharingUrl**</span></span> | `string` | <span data-ttu-id="7cf93-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cf93-122">Required.</span></span> <span data-ttu-id="7cf93-123">Маркер общего доступа, возвращенный API, или правильно закодированный URL-адрес для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="7cf93-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="7cf93-124">Кодирование URL-адресов для общего доступа</span><span class="sxs-lookup"><span data-stu-id="7cf93-124">Encoding sharing URLs</span></span>

<span data-ttu-id="7cf93-125">Чтобы закодировать URL-адрес для общего доступа, используйте следующую логику:</span><span class="sxs-lookup"><span data-stu-id="7cf93-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="7cf93-126">Для начала примените к URL-адресу кодировку base64.</span><span class="sxs-lookup"><span data-stu-id="7cf93-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="7cf93-127">Преобразуйте результат из кодировки base64 в [недополненный формат base64url](https://en.wikipedia.org/wiki/Base64), удалив символы `=` в конце значения и заменив `/` символом `_`, а `+` — символом `-`.)</span><span class="sxs-lookup"><span data-stu-id="7cf93-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="7cf93-128">Добавьте `u!` в начало строки.</span><span class="sxs-lookup"><span data-stu-id="7cf93-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="7cf93-129">Пример кодирования URL-адреса на C#:</span><span class="sxs-lookup"><span data-stu-id="7cf93-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a><span data-ttu-id="7cf93-130">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cf93-130">Optional request headers</span></span>

| <span data-ttu-id="7cf93-131">Имя</span><span class="sxs-lookup"><span data-stu-id="7cf93-131">Name</span></span>       | <span data-ttu-id="7cf93-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7cf93-132">Type</span></span>   | <span data-ttu-id="7cf93-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf93-133">Description</span></span>                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="7cf93-134">**Prefer**</span><span class="sxs-lookup"><span data-stu-id="7cf93-134">**Prefer**</span></span> | <span data-ttu-id="7cf93-135">string</span><span class="sxs-lookup"><span data-stu-id="7cf93-135">string</span></span> | <span data-ttu-id="7cf93-136">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7cf93-136">Optional.</span></span> <span data-ttu-id="7cf93-137">Установите одно из значений, `prefer` приведенных ниже.</span><span class="sxs-lookup"><span data-stu-id="7cf93-137">Set to one of the `prefer` values documented below.</span></span>  |

### <a name="prefer-header-values"></a><span data-ttu-id="7cf93-138">Предпочтительные значения заголовков</span><span class="sxs-lookup"><span data-stu-id="7cf93-138">Prefer header values</span></span>

| <span data-ttu-id="7cf93-139">Имя</span><span class="sxs-lookup"><span data-stu-id="7cf93-139">Name</span></span>                          | <span data-ttu-id="7cf93-140">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf93-140">Description</span></span>                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7cf93-141">Редимшаринглинк</span><span class="sxs-lookup"><span data-stu-id="7cf93-141">redeemSharingLink</span></span>             | <span data-ttu-id="7cf93-142">Если **шареидоренкодедшарингурл** представляет собой ссылку для совместного доступа, предоставьте вызывающему методу долговременный доступ к элементу</span><span class="sxs-lookup"><span data-stu-id="7cf93-142">If the **shareIdOrEncodedSharingUrl** is a sharing link, grant the caller durable access to the item</span></span>    |
| <span data-ttu-id="7cf93-143">Редимшаринглинкифнецессари</span><span class="sxs-lookup"><span data-stu-id="7cf93-143">redeemSharingLinkIfNecessary</span></span>  | <span data-ttu-id="7cf93-144">То же, что и Редимшаринглинк, но доступ гарантированно предоставляется только в течение этого запроса.</span><span class="sxs-lookup"><span data-stu-id="7cf93-144">Same as redeemSharingLink, but access is only guaranteed to be granted for the duration of this request</span></span> |

<span data-ttu-id="7cf93-145">Редимшаринглинк должен считаться эквивалентным участнику, который перемещается в ссылку для совместного доступа, в браузере (принимается жестом общего доступа), тогда как Редимшаринглинкифнецессари предназначено для сценариев, в которых намерением является просто взглянуть на ссылку метаданных.</span><span class="sxs-lookup"><span data-stu-id="7cf93-145">redeemSharingLink should be considered equivalent to the caller navigating to the sharing link the browser (accepting the sharing gesture), whereas redeemSharingLinkIfNecessary is intended for scenarios where the intention is simply to peek at the link's metadata.</span></span>

## <a name="response"></a><span data-ttu-id="7cf93-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cf93-146">Response</span></span>

<span data-ttu-id="7cf93-147">При успешном выполнении этот метод возвращает код отклика `200 OK` и ресурс [sharedDriveItem](../resources/shareddriveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7cf93-147">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cf93-148">Пример</span><span class="sxs-lookup"><span data-stu-id="7cf93-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cf93-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cf93-149">Request</span></span>

<span data-ttu-id="7cf93-150">Вот пример запроса для получения общего элемента:</span><span class="sxs-lookup"><span data-stu-id="7cf93-150">Here is an example of the request to retrieve a shared item:</span></span>

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a><span data-ttu-id="7cf93-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cf93-151">Response</span></span>

<span data-ttu-id="7cf93-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7cf93-152">Here is an example of the response.</span></span>

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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="7cf93-153">Прямой доступ к общему элементу</span><span class="sxs-lookup"><span data-stu-id="7cf93-153">Access the shared item directly</span></span>

<span data-ttu-id="7cf93-p104">Так как элемент [**SharedDriveItem**](../resources/shareddriveitem.md) содержит полезную информацию, большинство приложений будут стремиться получить прямой доступ к общему элементу [DriveItem](../resources/driveitem.md). Ресурс **SharedDriveItem** включает связи **корня** и **элементов**, которые могут получать доступ к содержимому в области общего элемента.</span><span class="sxs-lookup"><span data-stu-id="7cf93-p104">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="7cf93-156">Пример (один файл)</span><span class="sxs-lookup"><span data-stu-id="7cf93-156">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="7cf93-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cf93-157">Request</span></span>

<span data-ttu-id="7cf93-158">При запросе связи **driveItem** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="7cf93-158">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a><span data-ttu-id="7cf93-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="7cf93-159">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="7cf93-160">Пример (общая папка)</span><span class="sxs-lookup"><span data-stu-id="7cf93-160">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="7cf93-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cf93-161">Request</span></span>

<span data-ttu-id="7cf93-162">При запросе связи **driveItem** и расширении коллекции **children** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ, а также файлы, содержащиеся в общей папке.</span><span class="sxs-lookup"><span data-stu-id="7cf93-162">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a><span data-ttu-id="7cf93-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cf93-163">Response</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="7cf93-164">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="7cf93-164">Error Responses</span></span>

<span data-ttu-id="7cf93-165">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="7cf93-165">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="7cf93-166">Замечания</span><span class="sxs-lookup"><span data-stu-id="7cf93-166">Remarks</span></span>

* <span data-ttu-id="7cf93-167">В случае OneDrive для бизнеса и SharePoint API общих ресурсов всегда требует аутентификации. С его помощью невозможно обращаться к содержимому, доступ к которому предоставлен анонимно, без контекста пользователя.</span><span class="sxs-lookup"><span data-stu-id="7cf93-167">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link"
} -->
