---
title: Загрузить содержимое DriveItemVersion ресурсов
description: В этой статье рассказывается, как получить содержимое определенной версии ресурса DriveItem.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b6b1f8fbb840cba88f05cb30e2617ca23cb6ad1f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960842"
---
# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="1f0ee-103">Загрузить содержимое DriveItemVersion ресурсов</span><span class="sxs-lookup"><span data-stu-id="1f0ee-103">Download contents of a DriveItemVersion resource</span></span>

<span data-ttu-id="1f0ee-104">В этой статье рассказывается, как получить содержимое определенной версии ресурса [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1f0ee-104">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f0ee-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f0ee-105">Permissions</span></span>

<span data-ttu-id="1f0ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f0ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f0ee-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f0ee-108">Permission type</span></span>      | <span data-ttu-id="1f0ee-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f0ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f0ee-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f0ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f0ee-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f0ee-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f0ee-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f0ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f0ee-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f0ee-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f0ee-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f0ee-114">Application</span></span> | <span data-ttu-id="1f0ee-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f0ee-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="1f0ee-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f0ee-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="1f0ee-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f0ee-117">Response</span></span>

<span data-ttu-id="1f0ee-118">Возвращает отклик `302 Found`, который выполняет перенаправление на URL-адрес, прошедший предварительную проверку подлинности и предназначенный для скачивания байтов файла.</span><span class="sxs-lookup"><span data-stu-id="1f0ee-118">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="1f0ee-p102">Чтобы загрузить содержимое файла, приложению необходимо будет следовать заголовку `Location` в отклике. Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="1f0ee-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="1f0ee-121">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действуют только в течение короткого периода времени (несколько минут), и для их скачивания не требуется заголовок `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1f0ee-121">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="1f0ee-122">Пример</span><span class="sxs-lookup"><span data-stu-id="1f0ee-122">Example</span></span>

<span data-ttu-id="1f0ee-123">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="1f0ee-123">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="1f0ee-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f0ee-124">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="1f0ee-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f0ee-125">Response</span></span>

<span data-ttu-id="1f0ee-126">Возвращает перенаправление на расположение, из которого можно скачать содержимое версии.</span><span class="sxs-lookup"><span data-stu-id="1f0ee-126">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="1f0ee-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="1f0ee-127">Remarks</span></span>

<span data-ttu-id="1f0ee-128">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="1f0ee-128">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="1f0ee-129">Когда ваше приложение получает список доступных версий для файла, возвращается ресурс [DriveItemVersion](../resources/driveitemversion.md), в котором представлены доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="1f0ee-129">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
