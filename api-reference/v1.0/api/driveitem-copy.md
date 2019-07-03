---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Копирование файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a709c362ba8a37728479da01c20679d430b219e8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446033"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="937df-102">Копирование ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="937df-102">Copy a DriveItem</span></span>

<span data-ttu-id="937df-103">Асинхронно создает копию элемента [driveItem][item-resource] (включая все дочерние элементы) в новом родительском элементе или с новым именем.</span><span class="sxs-lookup"><span data-stu-id="937df-103">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="937df-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="937df-104">Permissions</span></span>

<span data-ttu-id="937df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937df-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="937df-107">Permission type</span></span>      | <span data-ttu-id="937df-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="937df-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="937df-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="937df-109">Delegated (work or school account)</span></span> | <span data-ttu-id="937df-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937df-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="937df-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="937df-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="937df-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937df-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="937df-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="937df-113">Application</span></span> | <span data-ttu-id="937df-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937df-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="937df-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="937df-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="937df-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="937df-116">Request body</span></span>

<span data-ttu-id="937df-117">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="937df-117">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="937df-118">Имя</span><span class="sxs-lookup"><span data-stu-id="937df-118">Name</span></span>            | <span data-ttu-id="937df-119">Значение</span><span class="sxs-lookup"><span data-stu-id="937df-119">Value</span></span>                                          | <span data-ttu-id="937df-120">Описание</span><span class="sxs-lookup"><span data-stu-id="937df-120">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="937df-121">parentReference</span><span class="sxs-lookup"><span data-stu-id="937df-121">parentReference</span></span> | [<span data-ttu-id="937df-122">ItemReference</span><span class="sxs-lookup"><span data-stu-id="937df-122">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="937df-p102">Необязательный. Отсылает к родительскому элементу, в котором будет создана копия.</span><span class="sxs-lookup"><span data-stu-id="937df-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="937df-125">name</span><span class="sxs-lookup"><span data-stu-id="937df-125">name</span></span>            | <span data-ttu-id="937df-126">string</span><span class="sxs-lookup"><span data-stu-id="937df-126">string</span></span>                                         | <span data-ttu-id="937df-p103">Необязательный. Новое имя копии. Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="937df-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="937df-130">**Примечание.** Элемент _parentReference_ должен включать параметры `driveId` и `id` для целевой папки.</span><span class="sxs-lookup"><span data-stu-id="937df-130">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="937df-131">Пример</span><span class="sxs-lookup"><span data-stu-id="937df-131">Example</span></span>

<span data-ttu-id="937df-132">В этом примере показано, как копировать файл с идентификатором `{item-id}` в папку с идентификатором `driveId` и значением `id`.</span><span class="sxs-lookup"><span data-stu-id="937df-132">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="937df-133">У новой копии файла будет имя `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="937df-133">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="937df-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="937df-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "tags": "service.graph", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "driveId": "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    "id": "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
  },
  "name": "contoso plan (copy).txt"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="937df-135">C#</span><span class="sxs-lookup"><span data-stu-id="937df-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="937df-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="937df-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="937df-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="937df-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="937df-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="937df-138">Response</span></span>

<span data-ttu-id="937df-139">Возвращает сведения о том, как [отслеживать ход](/graph/long-running-actions-overview) копирования после принятия запроса.</span><span class="sxs-lookup"><span data-stu-id="937df-139">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="937df-p105">В значении заголовка `Location` имеется URL-адрес службы, которая возвращает сведения о текущем состоянии операции копирования. Вы можете использовать эту информацию, чтобы [определить время окончания копирования](/graph/long-running-actions-overview).</span><span class="sxs-lookup"><span data-stu-id="937df-p105">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation. You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="937df-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="937df-142">Remarks</span></span>

<span data-ttu-id="937df-p106">Во многих случаях копирование выполняется асинхронно. Отклик API указывает, что операция копирования принята или отклонена, например из-за использования имени конечного файла.</span><span class="sxs-lookup"><span data-stu-id="937df-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
} -->
