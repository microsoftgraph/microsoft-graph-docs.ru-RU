---
title: Получение filesFolder
description: Получение пути навигации filesFolder канала.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8515b6ebb853c65ba44ce18c401179e115605689
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971288"
---
# <a name="get-filesfolder"></a><span data-ttu-id="15a95-103">Получение filesFolder</span><span class="sxs-lookup"><span data-stu-id="15a95-103">Get filesFolder</span></span>

<span data-ttu-id="15a95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15a95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15a95-105">Получайте метаданные для расположения, где хранятся файлы [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="15a95-105">Get the metadata for the location where the files of a [channel](../resources/channel.md) are stored.</span></span> 

## <a name="permissions"></a><span data-ttu-id="15a95-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15a95-106">Permissions</span></span>
<span data-ttu-id="15a95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15a95-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15a95-109">Permission type</span></span>      | <span data-ttu-id="15a95-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15a95-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15a95-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15a95-111">Delegated (work or school account)</span></span> | <span data-ttu-id="15a95-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15a95-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="15a95-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15a95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15a95-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15a95-114">Not supported.</span></span>    |
|<span data-ttu-id="15a95-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="15a95-115">Application</span></span> | <span data-ttu-id="15a95-116">File.Read.Group\*, Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15a95-116">File.Read.Group\*, Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="15a95-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="15a95-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="15a95-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15a95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15a95-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15a95-119">Optional query parameters</span></span>

<span data-ttu-id="15a95-120">Этот метод не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="15a95-120">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15a95-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15a95-121">Request headers</span></span>
| <span data-ttu-id="15a95-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15a95-122">Header</span></span>       | <span data-ttu-id="15a95-123">Значение</span><span class="sxs-lookup"><span data-stu-id="15a95-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="15a95-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15a95-124">Authorization</span></span>  | <span data-ttu-id="15a95-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15a95-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15a95-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15a95-127">Request body</span></span>
<span data-ttu-id="15a95-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15a95-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15a95-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="15a95-129">Response</span></span>

<span data-ttu-id="15a95-130">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="15a95-130">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15a95-131">Пример</span><span class="sxs-lookup"><span data-stu-id="15a95-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="15a95-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="15a95-132">Request</span></span>
<span data-ttu-id="15a95-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15a95-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15a95-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="15a95-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/filesFolder
```
# <a name="c"></a>[<span data-ttu-id="15a95-135">C#</span><span class="sxs-lookup"><span data-stu-id="15a95-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-filesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15a95-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15a95-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-filesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15a95-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15a95-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-filesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15a95-138">Java</span><span class="sxs-lookup"><span data-stu-id="15a95-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-filesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="15a95-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="15a95-139">Response</span></span>
<span data-ttu-id="15a95-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="15a95-140">The following is an example of the response.</span></span> 

><span data-ttu-id="15a95-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="15a95-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/channels('19%3Af253e46c035b42308e9a4a22a87037af%40thread.skype')/filesFolder/$entity",
    "id": "01H7CFEKENJSSIUHGADZBKODARINQC5JMD",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "2020-01-23T18:47:13Z",
    "lastEditedDateTime": null,
    "name": "Documentation Planning",
    "webUrl": "https://microsoft.sharepoint.com/teams/ExtensibilityandFundamentals/Shared%20Documents/Documentation%20Planning",
    "size": 2374080,
    "parentReference": {
        "driveId": "b!2SInBlQrN0K8-GXMy9qNsPtI5ScW8C5IlZtycoy6ZpJZRRtgE4qVTrE8wrvL0-hd",
        "driveType": "documentLibrary"
    },
    "fileSystemInfo": {
        "createdDateTime": "2020-01-23T18:47:12Z",
        "lastModifiedDateTime": "2020-01-23T18:47:13Z",
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



