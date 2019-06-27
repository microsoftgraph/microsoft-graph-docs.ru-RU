---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Загрузка предыдущей версии
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 55bc0d029cd64e420b956c41f10f3786a62cce88
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259992"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="c9949-102">Скачивание содержимого ресурса DriveItemVersion (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="c9949-102">Download contents of a DriveItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9949-103">Получение содержимого определенной версии [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c9949-103">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="c9949-104">**Примечание:** Не поддерживается извлечение контента текущей версии.</span><span class="sxs-lookup"><span data-stu-id="c9949-104">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="c9949-105">Вместо этого используйте [конечную точку содержимого driveItem](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="c9949-105">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9949-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9949-106">Permissions</span></span>

<span data-ttu-id="c9949-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9949-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9949-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9949-109">Permission type</span></span>      | <span data-ttu-id="c9949-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9949-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9949-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9949-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9949-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9949-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9949-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9949-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9949-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9949-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9949-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9949-115">Application</span></span> | <span data-ttu-id="c9949-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9949-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="c9949-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9949-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="c9949-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9949-118">Response</span></span>

<span data-ttu-id="c9949-119">Возвращает отклик `302 Found`, который выполняет перенаправление на URL-адрес, прошедший предварительную проверку подлинности и предназначенный для скачивания байтов файла.</span><span class="sxs-lookup"><span data-stu-id="c9949-119">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="c9949-p103">Чтобы загрузить содержимое файла, приложению необходимо будет следовать заголовку `Location` в отклике. Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="c9949-p103">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="c9949-122">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действуют только в течение короткого периода времени (несколько минут), и для их скачивания не требуется заголовок `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c9949-122">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="c9949-123">Пример</span><span class="sxs-lookup"><span data-stu-id="c9949-123">Example</span></span>

<span data-ttu-id="c9949-124">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="c9949-124">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="c9949-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9949-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="c9949-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9949-126">Response</span></span>

<span data-ttu-id="c9949-127">Возвращает перенаправление на расположение, из которого можно скачать содержимое версии.</span><span class="sxs-lookup"><span data-stu-id="c9949-127">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c9949-128">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c9949-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c9949-129">C#</span><span class="sxs-lookup"><span data-stu-id="c9949-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-version-contents-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9949-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="c9949-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-version-contents-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c9949-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c9949-131">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-version-contents-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="remarks"></a><span data-ttu-id="c9949-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="c9949-132">Remarks</span></span>

<span data-ttu-id="c9949-133">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="c9949-133">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="c9949-134">Когда приложение извлекает список доступных версий для файла, возвращается ресурс [driveItemVersion](../resources/driveitemversion.md) , который предоставляет доступ к сведениям о конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="c9949-134">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitemversion-get-contents.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
