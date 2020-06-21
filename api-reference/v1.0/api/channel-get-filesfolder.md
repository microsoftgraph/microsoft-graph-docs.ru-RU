---
title: Получение Филесфолдер
description: Получение Филесфолдер канала.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3701c0fde058f0040f1d4a25f882516a022893ea
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788442"
---
# <a name="get-filesfolder"></a><span data-ttu-id="0b04d-103">Получение Филесфолдер</span><span class="sxs-lookup"><span data-stu-id="0b04d-103">Get filesFolder</span></span>

<span data-ttu-id="0b04d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b04d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b04d-105">Получение пути навигации Филесфолдер, который представляет собой метаданные для расположения, в котором хранятся файлы канала, для [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="0b04d-105">Retrieve the filesFolder navigation path, which is the metadata for the location where the channel files are stored, for a [channel](../resources/channel.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="0b04d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b04d-106">Permissions</span></span>
<span data-ttu-id="0b04d-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0b04d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0b04d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b04d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b04d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b04d-109">Permission type</span></span>      | <span data-ttu-id="0b04d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b04d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b04d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b04d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b04d-112">File. Read. ALL, Group. Read. ALL, File. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b04d-112">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0b04d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b04d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b04d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b04d-114">Not supported.</span></span>    |
|<span data-ttu-id="0b04d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b04d-115">Application</span></span> | <span data-ttu-id="0b04d-116">File. Read. ALL, Group. Read. ALL, File. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b04d-116">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>     |


## <a name="http-request"></a><span data-ttu-id="0b04d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b04d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder

```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b04d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b04d-118">Optional query parameters</span></span>

<span data-ttu-id="0b04d-119">Этот метод не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0b04d-119">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b04d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b04d-120">Request headers</span></span>
| <span data-ttu-id="0b04d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b04d-121">Header</span></span>       | <span data-ttu-id="0b04d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b04d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b04d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b04d-123">Authorization</span></span>  | <span data-ttu-id="0b04d-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0b04d-124">Bearer {token}.</span></span> <span data-ttu-id="0b04d-125">Required.</span><span class="sxs-lookup"><span data-stu-id="0b04d-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b04d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b04d-126">Request body</span></span>
<span data-ttu-id="0b04d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b04d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b04d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b04d-128">Response</span></span>

<span data-ttu-id="0b04d-129">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b04d-129">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b04d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0b04d-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b04d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b04d-131">Request</span></span>

<span data-ttu-id="0b04d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b04d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/filesFolder
```
### <a name="response"></a><span data-ttu-id="0b04d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b04d-133">Response</span></span>

<span data-ttu-id="0b04d-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b04d-134">The following is an example of the response.</span></span> 

><span data-ttu-id="0b04d-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0b04d-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b04d-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0b04d-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/channels('19%3Af253e46c035b42308e9a4a22a87037af%40thread.skype')/filesFolder/$entity",
    "id": "01H7CFEKENJSSIUHGADZBKODARINQC5JMD",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "2020-01-23T18:47:13Z",
    "name": "Documentation Planning",
    "webUrl": "https://microsoft.sharepoint.com/teams/ExtensibilityandFundamentals/Shared%20Documents/Documentation%20Planning",
    "size": 2374080,
    "parentReference": {
        "driveId": "b!2SInBlQrN0K8-GXMy9qNsPtI5ScW8C5IlZtycoy6ZpJZRRtgE4qVTrE8wrvL0-hd",
        "driveType": "documentLibrary"
    },
    "fileSystemInfo": {
        "createdDateTime": "2020-01-23T18:47:12Z",
        "lastModifiedDateTime": "2020-01-23T18:47:13Z"
    },
    "folder": {
        "childCount": 7
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get filesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
