---
author: JeremyKelley
description: Асинхронно создает копию объекта [driveItem] [Item-Resource] (включая все дочерние элементы) в новом родительском элементе или с новым именем.
ms.date: 09/10/2017
title: Копирование файла или папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2c4c95e90a81d5336914b3638119f4802f86aea1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982145"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="afb9c-103">Копирование ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="afb9c-103">Copy a DriveItem</span></span>

<span data-ttu-id="afb9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afb9c-105">Асинхронно создает копию элемента [driveItem][item-resource] (включая все дочерние элементы) в новом родительском элементе или с новым именем.</span><span class="sxs-lookup"><span data-stu-id="afb9c-105">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="afb9c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afb9c-106">Permissions</span></span>

<span data-ttu-id="afb9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afb9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afb9c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afb9c-109">Permission type</span></span>      | <span data-ttu-id="afb9c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afb9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afb9c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afb9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="afb9c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb9c-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="afb9c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afb9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afb9c-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb9c-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="afb9c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afb9c-115">Application</span></span> | <span data-ttu-id="afb9c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb9c-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afb9c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afb9c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="afb9c-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="afb9c-118">Request body</span></span>

<span data-ttu-id="afb9c-119">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="afb9c-119">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="afb9c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="afb9c-120">Name</span></span>            | <span data-ttu-id="afb9c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="afb9c-121">Value</span></span>                                          | <span data-ttu-id="afb9c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="afb9c-122">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="afb9c-123">parentReference</span><span class="sxs-lookup"><span data-stu-id="afb9c-123">parentReference</span></span> | [<span data-ttu-id="afb9c-124">ItemReference</span><span class="sxs-lookup"><span data-stu-id="afb9c-124">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="afb9c-p102">Необязательный. Отсылает к родительскому элементу, в котором будет создана копия.</span><span class="sxs-lookup"><span data-stu-id="afb9c-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="afb9c-127">name</span><span class="sxs-lookup"><span data-stu-id="afb9c-127">name</span></span>            | <span data-ttu-id="afb9c-128">string</span><span class="sxs-lookup"><span data-stu-id="afb9c-128">string</span></span>                                         | <span data-ttu-id="afb9c-p103">Необязательный. Новое имя копии. Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="afb9c-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="afb9c-132">**Примечание.** Элемент _parentReference_ должен включать параметры `driveId` и `id` для целевой папки.</span><span class="sxs-lookup"><span data-stu-id="afb9c-132">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="afb9c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="afb9c-133">Example</span></span>

<span data-ttu-id="afb9c-134">В этом примере показано, как копировать файл с идентификатором `{item-id}` в папку с идентификатором `driveId` и значением `id`.</span><span class="sxs-lookup"><span data-stu-id="afb9c-134">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="afb9c-135">У новой копии файла будет имя `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="afb9c-135">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>


# <a name="http"></a>[<span data-ttu-id="afb9c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="afb9c-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite", "target": "action" } -->

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
# <a name="c"></a>[<span data-ttu-id="afb9c-137">C#</span><span class="sxs-lookup"><span data-stu-id="afb9c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/copy-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afb9c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afb9c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/copy-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afb9c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afb9c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/copy-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="afb9c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="afb9c-140">Response</span></span>

<span data-ttu-id="afb9c-141">Возвращает сведения о том, как [отслеживать ход](/graph/long-running-actions-overview) копирования после принятия запроса.</span><span class="sxs-lookup"><span data-stu-id="afb9c-141">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="afb9c-p105">В значении заголовка `Location` имеется URL-адрес службы, которая возвращает сведения о текущем состоянии операции копирования. Вы можете использовать эту информацию, чтобы [определить время окончания копирования](/graph/long-running-actions-overview).</span><span class="sxs-lookup"><span data-stu-id="afb9c-p105">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation. You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="afb9c-144">Замечания</span><span class="sxs-lookup"><span data-stu-id="afb9c-144">Remarks</span></span>

<span data-ttu-id="afb9c-p106">Во многих случаях копирование выполняется асинхронно. Отклик API указывает, что операция копирования принята или отклонена, например из-за использования имени конечного файла.</span><span class="sxs-lookup"><span data-stu-id="afb9c-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->


