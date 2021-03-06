---
author: JeremyKelley
description: 'Извлечение содержимого определенной версии driveItem. '
ms.date: 09/10/2017
title: Загрузка предыдущей версии
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c521c3ad4c4776e67747d9f6b09deb5e39fcac82
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515529"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="d3e9e-103">Скачивание содержимого ресурса DriveItemVersion (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-103">Download contents of a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="d3e9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3e9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3e9e-105">Извлечение содержимого определенной версии [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d3e9e-105">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="d3e9e-106">**Примечание:** Получение контента текущей версии не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-106">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="d3e9e-107">Вместо этого используйте [конечную точку контента driveItem.](driveitem-get-content.md)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-107">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3e9e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3e9e-108">Permissions</span></span>

<span data-ttu-id="d3e9e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e9e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3e9e-111">Permission type</span></span>      | <span data-ttu-id="d3e9e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3e9e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d3e9e-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e9e-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3e9e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3e9e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3e9e-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e9e-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3e9e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3e9e-117">Application</span></span> | <span data-ttu-id="d3e9e-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e9e-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="d3e9e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3e9e-119">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/items/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="d3e9e-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3e9e-120">Response</span></span>

<span data-ttu-id="d3e9e-121">Возвращает отклик `302 Found`, который выполняет перенаправление на URL-адрес, прошедший предварительную проверку подлинности и предназначенный для скачивания байтов файла.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-121">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="d3e9e-p103">Чтобы загрузить содержимое файла, приложению необходимо будет следовать заголовку `Location` в отклике. Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-p103">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="d3e9e-124">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действуют только в течение короткого периода времени (несколько минут), и для их скачивания не требуется заголовок `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-124">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="d3e9e-125">Пример</span><span class="sxs-lookup"><span data-stu-id="d3e9e-125">Example</span></span>

<span data-ttu-id="d3e9e-126">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-126">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="d3e9e-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3e9e-127">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d3e9e-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e9e-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/versions/{version-id}/content
```
# <a name="c"></a>[<span data-ttu-id="d3e9e-129">C#</span><span class="sxs-lookup"><span data-stu-id="d3e9e-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-version-contents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3e9e-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3e9e-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-version-contents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3e9e-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3e9e-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-version-contents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3e9e-132">Java</span><span class="sxs-lookup"><span data-stu-id="d3e9e-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-version-contents-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3e9e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3e9e-133">Response</span></span>

<span data-ttu-id="d3e9e-134">Возвращает перенаправление на расположение, из которого можно скачать содержимое версии.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-134">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="d3e9e-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="d3e9e-135">Remarks</span></span>

<span data-ttu-id="d3e9e-136">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-136">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="d3e9e-137">Когда приложение извлекает список доступных версий для файла, возвращается ресурс [driveItemVersion,](../resources/driveitemversion.md) который предоставляет доступную информацию о конкретной версии.</span><span class="sxs-lookup"><span data-stu-id="d3e9e-137">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
  ]
}
-->


