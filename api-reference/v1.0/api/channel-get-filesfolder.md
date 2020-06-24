---
title: Получение Филесфолдер
description: Получение Филесфолдер канала.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0190f09eacb08dccdb5f8297fb3e7011cacaa0a0
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845668"
---
# <a name="get-filesfolder"></a><span data-ttu-id="92ea7-103">Получение Филесфолдер</span><span class="sxs-lookup"><span data-stu-id="92ea7-103">Get filesFolder</span></span>

<span data-ttu-id="92ea7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92ea7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92ea7-105">Получение метаданных для расположения, в котором хранятся файлы [канала](../resources/channel.md) .</span><span class="sxs-lookup"><span data-stu-id="92ea7-105">Get the metadata for the location where the files of a [channel](../resources/channel.md) are stored.</span></span> 

## <a name="permissions"></a><span data-ttu-id="92ea7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92ea7-106">Permissions</span></span>
<span data-ttu-id="92ea7-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="92ea7-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="92ea7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ea7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ea7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92ea7-109">Permission type</span></span>      | <span data-ttu-id="92ea7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92ea7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92ea7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92ea7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="92ea7-112">File. Read. ALL, Group. Read. ALL, File. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="92ea7-112">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="92ea7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92ea7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ea7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92ea7-114">Not supported.</span></span>    |
|<span data-ttu-id="92ea7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92ea7-115">Application</span></span> | <span data-ttu-id="92ea7-116">File. Read. ALL, Group. Read. ALL, File. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="92ea7-116">File.Read.All, Group.Read.All, File.ReadWrite.All, Group.ReadWrite.All</span></span>     |


## <a name="http-request"></a><span data-ttu-id="92ea7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92ea7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder

```

## <a name="optional-query-parameters"></a><span data-ttu-id="92ea7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="92ea7-118">Optional query parameters</span></span>

<span data-ttu-id="92ea7-119">Этот метод не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="92ea7-119">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92ea7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92ea7-120">Request headers</span></span>
| <span data-ttu-id="92ea7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92ea7-121">Header</span></span>       | <span data-ttu-id="92ea7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="92ea7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92ea7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92ea7-123">Authorization</span></span>  | <span data-ttu-id="92ea7-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="92ea7-124">Bearer {token}.</span></span> <span data-ttu-id="92ea7-125">Required.</span><span class="sxs-lookup"><span data-stu-id="92ea7-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92ea7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="92ea7-126">Request body</span></span>
<span data-ttu-id="92ea7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92ea7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92ea7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="92ea7-128">Response</span></span>

<span data-ttu-id="92ea7-129">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="92ea7-129">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ea7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="92ea7-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="92ea7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="92ea7-131">Request</span></span>

<span data-ttu-id="92ea7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92ea7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/filesFolder
```
### <a name="response"></a><span data-ttu-id="92ea7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="92ea7-133">Response</span></span>

<span data-ttu-id="92ea7-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92ea7-134">The following is an example of the response.</span></span> 

><span data-ttu-id="92ea7-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="92ea7-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="92ea7-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="92ea7-136">All the properties will be returned from an actual call.</span></span>
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
