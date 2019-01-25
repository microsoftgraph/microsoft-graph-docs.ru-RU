---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Копирование файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 378f47d380e6d144791d3551a398d1dcd0886295
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517556"
---
# <a name="copy-a-driveitem"></a><span data-ttu-id="ad7d6-102">Копирование ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="ad7d6-102">Copy a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad7d6-103">Асинхронно создает копию элемента [driveItem][item-resource] (включая все дочерние элементы) в новом родительском элементе или с новым именем.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-103">Asynchronously creates a copy of an [driveItem][item-resource] (including any children), under a new parent item or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad7d6-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad7d6-104">Permissions</span></span>

<span data-ttu-id="ad7d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad7d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad7d6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad7d6-107">Permission type</span></span>      | <span data-ttu-id="ad7d6-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad7d6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad7d6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad7d6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ad7d6-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad7d6-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad7d6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad7d6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad7d6-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad7d6-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ad7d6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad7d6-113">Application</span></span> | <span data-ttu-id="ad7d6-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad7d6-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad7d6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad7d6-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/copy
POST /groups/{groupId}/drive/items/{itemId}/copy
POST /me/drive/items/{item-id}/copy
POST /sites/{siteId}/drive/items/{itemId}/copy
POST /users/{userId}/drive/items/{itemId}/copy
```

### <a name="request-body"></a><span data-ttu-id="ad7d6-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad7d6-116">Request body</span></span>

<span data-ttu-id="ad7d6-117">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-117">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="ad7d6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ad7d6-118">Name</span></span>            | <span data-ttu-id="ad7d6-119">Значение</span><span class="sxs-lookup"><span data-stu-id="ad7d6-119">Value</span></span>                                          | <span data-ttu-id="ad7d6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ad7d6-120">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ad7d6-121">parentReference</span><span class="sxs-lookup"><span data-stu-id="ad7d6-121">parentReference</span></span> | [<span data-ttu-id="ad7d6-122">ItemReference</span><span class="sxs-lookup"><span data-stu-id="ad7d6-122">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="ad7d6-p102">Необязательный. Отсылает к родительскому элементу, в котором будет создана копия.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="ad7d6-125">name</span><span class="sxs-lookup"><span data-stu-id="ad7d6-125">name</span></span>            | <span data-ttu-id="ad7d6-126">строка</span><span class="sxs-lookup"><span data-stu-id="ad7d6-126">string</span></span>                                         | <span data-ttu-id="ad7d6-p103">Необязательный. Новое имя копии. Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="ad7d6-130">**Примечание.** Элемент _parentReference_ должен включать параметры `driveId` и `id` для целевой папки.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-130">**Note:** The _parentReference_ should include the `driveId` and `id` parameters for the target folder.</span></span>

## <a name="example"></a><span data-ttu-id="ad7d6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ad7d6-131">Example</span></span>

<span data-ttu-id="ad7d6-132">В этом примере показано, как копировать файл с идентификатором `{item-id}` в папку с идентификатором `driveId` и значением `id`.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-132">This example copies a file identified by `{item-id}` into a folder identified with a `driveId` and `id` value.</span></span>
<span data-ttu-id="ad7d6-133">У новой копии файла будет имя `contoso plan (copy).txt`.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-133">The new copy of the file will be named `contoso plan (copy).txt`.</span></span>

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

## <a name="response"></a><span data-ttu-id="ad7d6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad7d6-134">Response</span></span>

<span data-ttu-id="ad7d6-135">Возвращает сведения о том, как [отслеживать ход](/graph/long-running-actions-overview) копирования после принятия запроса.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-135">Returns details about how to [monitor the progress](/graph/long-running-actions-overview) of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://contoso.sharepoint.com/_api/v2.0/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="ad7d6-136">В значении заголовка `Location` имеется URL-адрес службы, которая возвращает сведения о текущем состоянии операции копирования.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-136">The value of the `Location` header provides a URL for a service that will return the current state of the copy operation.</span></span>
<span data-ttu-id="ad7d6-137">Вы можете использовать эти сведения, чтобы [определить, когда копирование будет завершено](/graph/long-running-actions-overview).</span><span class="sxs-lookup"><span data-stu-id="ad7d6-137">You can use this info to [determine when the copy has finished](/graph/long-running-actions-overview).</span></span>

### <a name="remarks"></a><span data-ttu-id="ad7d6-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="ad7d6-138">Remarks</span></span>

<span data-ttu-id="ad7d6-p106">Во многих случаях копирование выполняется асинхронно. Отклик API указывает, что операция копирования принята или отклонена, например из-за использования имени конечного файла.</span><span class="sxs-lookup"><span data-stu-id="ad7d6-p106">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-copy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
