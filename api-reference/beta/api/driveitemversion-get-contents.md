---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Загрузите предыдущей версии
ms.openlocfilehash: 1d55a457060197cfd9a24a39506003518918d398
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075683"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="ebcf7-102">Скачивание содержимого ресурса DriveItemVersion (ознакомительная версия)</span><span class="sxs-lookup"><span data-stu-id="ebcf7-102">Download contents of a DriveItemVersion resource (preview)</span></span>

> <span data-ttu-id="ebcf7-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebcf7-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebcf7-105">Извлечение содержимого части определенной версии [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ebcf7-105">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="ebcf7-106">**Примечание:** Получение содержимого текущей версии не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-106">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="ebcf7-107">Используйте [driveItem контента конечной точки](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="ebcf7-107">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ebcf7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebcf7-108">Permissions</span></span>

<span data-ttu-id="ebcf7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebcf7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcf7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebcf7-111">Permission type</span></span>      | <span data-ttu-id="ebcf7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebcf7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebcf7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebcf7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ebcf7-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcf7-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ebcf7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebcf7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcf7-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcf7-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ebcf7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebcf7-117">Application</span></span> | <span data-ttu-id="ebcf7-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebcf7-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="ebcf7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebcf7-119">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="ebcf7-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebcf7-120">Response</span></span>

<span data-ttu-id="ebcf7-121">Возвращает отклик `302 Found`, который выполняет перенаправление на URL-адрес, прошедший предварительную проверку подлинности и предназначенный для скачивания байтов файла.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-121">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="ebcf7-p104">Чтобы загрузить содержимое файла, приложению необходимо будет следовать заголовку `Location` в отклике. Многие библиотеки клиентов HTTP будут автоматически следовать перенаправлению 302 и немедленно начинать загрузку файла.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="ebcf7-124">URL-адреса загрузки, прошедшие предварительную проверку подлинности, действуют только в течение короткого периода времени (несколько минут), и для их скачивания не требуется заголовок `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-124">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="ebcf7-125">Пример</span><span class="sxs-lookup"><span data-stu-id="ebcf7-125">Example</span></span>

<span data-ttu-id="ebcf7-126">В этом примере показано, как получить версию файла в объекте drive текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-126">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="ebcf7-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebcf7-127">Request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="ebcf7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebcf7-128">Response</span></span>

<span data-ttu-id="ebcf7-129">Возвращает перенаправление на расположение, из которого можно скачать содержимое версии.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-129">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="ebcf7-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="ebcf7-130">Remarks</span></span>

<span data-ttu-id="ebcf7-131">OneDrive не сохраняет полные метаданные для предыдущих версий файла.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="ebcf7-132">Если ваше приложение получает список доступных версий файла, [driveItemVersion](../resources/driveitemversion.md) ресурсов возвращается, предоставляющий доступные сведения об определенной версии.</span><span class="sxs-lookup"><span data-stu-id="ebcf7-132">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
