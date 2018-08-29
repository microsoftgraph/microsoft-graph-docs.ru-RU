---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Доступ к общим элементам
ms.openlocfilehash: 4566452cc661d9ad2c913c06333a56bfcb0d5fce
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268272"
---
# <a name="accessing-shared-driveitems"></a><span data-ttu-id="11028-102">Доступ к общим элементам DriveItem</span><span class="sxs-lookup"><span data-stu-id="11028-102">Accessing shared DriveItems</span></span>

<span data-ttu-id="11028-103">Вы можете получить доступ к общим элементам [DriveItem](../resources/driveitem.md) или коллекции общих элементов, используя параметр **shareId** или URL-адрес для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="11028-103">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="11028-104">Чтобы использовать URL-адрес для совместного доступа с этим API, вашему приложению необходимо [преобразовать URL-адрес в токен общего доступа](#encoding-sharing-urls).</span><span class="sxs-lookup"><span data-stu-id="11028-104">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#encoding-sharing-urls).</span></span>

## <a name="permissions"></a><span data-ttu-id="11028-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11028-105">Permissions</span></span>

<span data-ttu-id="11028-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="11028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="11028-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11028-108">Permission type</span></span>      | <span data-ttu-id="11028-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11028-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11028-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11028-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11028-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11028-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="11028-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11028-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11028-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11028-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="11028-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11028-114">Application</span></span> | <span data-ttu-id="11028-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11028-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11028-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11028-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a><span data-ttu-id="11028-117">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="11028-117">Path Parameters</span></span>

| <span data-ttu-id="11028-118">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="11028-118">Parameter Name</span></span>        | <span data-ttu-id="11028-119">Значение</span><span class="sxs-lookup"><span data-stu-id="11028-119">Value</span></span>    | <span data-ttu-id="11028-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11028-120">Description</span></span>                                                                         |
|:----------------------|:---------|:------------------------------------------------------------------------------------|
| <span data-ttu-id="11028-121">**sharingTokenOrUrl**</span><span class="sxs-lookup"><span data-stu-id="11028-121">**sharingTokenOrUrl**</span></span> | `string` | <span data-ttu-id="11028-122">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11028-122">Required.</span></span> <span data-ttu-id="11028-123">Маркер общего доступа, возвращенный API, или правильно закодированный URL-адрес для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="11028-123">A sharing token as returned by the API or a properly encoded sharing URL.</span></span> |

### <a name="encoding-sharing-urls"></a><span data-ttu-id="11028-124">Кодирование URL-адресов для общего доступа</span><span class="sxs-lookup"><span data-stu-id="11028-124">Encoding sharing URLs</span></span>

<span data-ttu-id="11028-125">Чтобы закодировать URL-адрес для общего доступа, используйте следующую логику:</span><span class="sxs-lookup"><span data-stu-id="11028-125">To encode a sharing URL, use the following logic:</span></span>

1. <span data-ttu-id="11028-126">Для начала примените к URL-адресу кодировку base64.</span><span class="sxs-lookup"><span data-stu-id="11028-126">First, use base64 encode the URL.</span></span>
2. <span data-ttu-id="11028-127">Преобразуйте результат из кодировки base64 в [недополненный формат base64url](https://en.wikipedia.org/wiki/Base64), удалив символы `=` в конце значения и заменив `/` символом `_`, а `+` — символом `-`.)</span><span class="sxs-lookup"><span data-stu-id="11028-127">Convert the base64 encoded result to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by removing `=` characters from the end of the value, replacing `/` with `_` and `+` with `-`.)</span></span>
3. <span data-ttu-id="11028-128">Добавьте `u!` в начало строки.</span><span class="sxs-lookup"><span data-stu-id="11028-128">Append `u!` to be beginning of the string.</span></span>

<span data-ttu-id="11028-129">Ниже показан пример кодирования URL-адреса в языке C#:</span><span class="sxs-lookup"><span data-stu-id="11028-129">As an example, to encode a URL in C#:</span></span>

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="response"></a><span data-ttu-id="11028-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="11028-130">Response</span></span>

<span data-ttu-id="11028-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и ресурс [sharedDriveItem](../resources/shareddriveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11028-131">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11028-132">Пример</span><span class="sxs-lookup"><span data-stu-id="11028-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="11028-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="11028-133">Request</span></span>

<span data-ttu-id="11028-134">Вот пример запроса для получения общего элемента:</span><span class="sxs-lookup"><span data-stu-id="11028-134">Here is an example of the request to retrieve a shared item:</span></span>

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a><span data-ttu-id="11028-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="11028-135">Response</span></span>

<span data-ttu-id="11028-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11028-136">Here is an example of the response.</span></span>

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

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="11028-137">Прямой доступ к общему элементу</span><span class="sxs-lookup"><span data-stu-id="11028-137">Access the shared item directly</span></span>

<span data-ttu-id="11028-p103">Так как элемент [**SharedDriveItem**](../resources/shareddriveitem.md) содержит полезную информацию, большинство приложений будут стремиться получить прямой доступ к общему элементу [DriveItem](../resources/driveitem.md). Ресурс **SharedDriveItem** включает связи **корня** и **элементов**, которые могут получать доступ к содержимому в области общего элемента.</span><span class="sxs-lookup"><span data-stu-id="11028-p103">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="11028-140">Пример (один файл)</span><span class="sxs-lookup"><span data-stu-id="11028-140">Example (single file)</span></span>

### <a name="request"></a><span data-ttu-id="11028-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="11028-141">Request</span></span>

<span data-ttu-id="11028-142">При запросе связи **driveItem** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="11028-142">By requesting the **driveItem** relationship, the **DriveItem** that was shared will be returned.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a><span data-ttu-id="11028-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="11028-143">Response</span></span>

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

## <a name="example-shared-folder"></a><span data-ttu-id="11028-144">Пример (общая папка)</span><span class="sxs-lookup"><span data-stu-id="11028-144">Example (shared folder)</span></span>

### <a name="request"></a><span data-ttu-id="11028-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="11028-145">Request</span></span>

<span data-ttu-id="11028-146">При запросе связи **driveItem** и расширении коллекции **children** будет возвращен элемент **DriveItem**, к которому предоставлен общий доступ, а также файлы, содержащиеся в общей папке.</span><span class="sxs-lookup"><span data-stu-id="11028-146">By requesting the **driveItem** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a><span data-ttu-id="11028-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="11028-147">Response</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="11028-148">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="11028-148">Error Responses</span></span>

<span data-ttu-id="11028-149">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="11028-149">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="remarks"></a><span data-ttu-id="11028-150">Замечания</span><span class="sxs-lookup"><span data-stu-id="11028-150">Remarks</span></span>

* <span data-ttu-id="11028-151">В случае OneDrive для бизнеса и SharePoint API общих ресурсов всегда требует аутентификации. С его помощью невозможно обращаться к содержимому, доступ к которому предоставлен анонимно, без контекста пользователя.</span><span class="sxs-lookup"><span data-stu-id="11028-151">For OneDrive for Business and SharePoint, the Shares API always requires authentication and cannot be used to access anonymously shared content without a user context.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link"
} -->
