---
title: Получение filesFolder
description: Получение filesFolder канала.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 32272d197ff46545a7152f72f660a6132486d6c0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039897"
---
# <a name="get-filesfolder"></a><span data-ttu-id="5431e-103">Получение filesFolder</span><span class="sxs-lookup"><span data-stu-id="5431e-103">Get filesFolder</span></span>

<span data-ttu-id="5431e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5431e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5431e-105">Получайте метаданные для расположения, где хранятся файлы [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="5431e-105">Get the metadata for the location where the files of a [channel](../resources/channel.md) are stored.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5431e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5431e-106">Permissions</span></span>
<span data-ttu-id="5431e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5431e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5431e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5431e-109">Permission type</span></span>      | <span data-ttu-id="5431e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5431e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5431e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5431e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5431e-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5431e-112">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="5431e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5431e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5431e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5431e-114">Not supported.</span></span>    |
|<span data-ttu-id="5431e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5431e-115">Application</span></span> | <span data-ttu-id="5431e-116">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5431e-116">Files.Read.All, Files.ReadWrite.All, Group.Read.All, Group.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="5431e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5431e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/filesFolder
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5431e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5431e-118">Optional query parameters</span></span>

<span data-ttu-id="5431e-119">Этот метод не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5431e-119">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5431e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5431e-120">Request headers</span></span>
| <span data-ttu-id="5431e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5431e-121">Header</span></span>       | <span data-ttu-id="5431e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5431e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5431e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5431e-123">Authorization</span></span>  | <span data-ttu-id="5431e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5431e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5431e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5431e-126">Request body</span></span>
<span data-ttu-id="5431e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5431e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5431e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5431e-128">Response</span></span>

<span data-ttu-id="5431e-129">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5431e-129">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5431e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5431e-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="5431e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5431e-131">Request</span></span>

<span data-ttu-id="5431e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5431e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5431e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5431e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_filesFolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/filesFolder
```
# <a name="c"></a>[<span data-ttu-id="5431e-134">C#</span><span class="sxs-lookup"><span data-stu-id="5431e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-filesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5431e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5431e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-filesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5431e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5431e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-filesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5431e-137">Java</span><span class="sxs-lookup"><span data-stu-id="5431e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-filesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5431e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5431e-138">Response</span></span>

<span data-ttu-id="5431e-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5431e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="5431e-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5431e-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

