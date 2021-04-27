---
title: 'блокнот: getNotebookFromWebUrl'
description: Извлечение свойств и связей объекта записной книжки с помощью url-адреса.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 25c0731270edd5576ab2416682a6e6395b0e41b9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049242"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="b1676-103">блокнот: getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="b1676-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="b1676-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1676-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1676-105">Извлечение свойств и связей объекта [записной книжки](../resources/notebook.md) с помощью url-адреса.</span><span class="sxs-lookup"><span data-stu-id="b1676-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="b1676-106">Расположение может быть пользовательскими записными книжками в Microsoft 365, групповых записных книжках или SharePoint записных книжках Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b1676-106">The location can be user notebooks on Microsoft 365, group notebooks, or SharePoint site-hosted team notebooks on Microsoft 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="b1676-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1676-107">Permissions</span></span>
<span data-ttu-id="b1676-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1676-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1676-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1676-110">Permission type</span></span>      | <span data-ttu-id="b1676-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1676-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1676-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1676-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1676-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1676-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1676-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1676-114">Application</span></span> | <span data-ttu-id="b1676-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1676-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1676-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1676-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="b1676-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1676-117">Request headers</span></span>
| <span data-ttu-id="b1676-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b1676-118">Name</span></span>       | <span data-ttu-id="b1676-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b1676-119">Type</span></span> | <span data-ttu-id="b1676-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b1676-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1676-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1676-121">Authorization</span></span>  | <span data-ttu-id="b1676-122">string</span><span class="sxs-lookup"><span data-stu-id="b1676-122">string</span></span>  | <span data-ttu-id="b1676-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1676-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1676-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1676-125">Accept</span></span> | <span data-ttu-id="b1676-126">строка</span><span class="sxs-lookup"><span data-stu-id="b1676-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b1676-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1676-127">Request body</span></span>
<span data-ttu-id="b1676-128">В тексте запроса поставляем представление JSON полного URL-адреса в ноутбук, который необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="b1676-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="b1676-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1676-129">Property</span></span>     | <span data-ttu-id="b1676-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b1676-130">Type</span></span>        | <span data-ttu-id="b1676-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b1676-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="b1676-132">Путь URL-адреса для получения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="b1676-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="b1676-133">Он также может содержать префикс "onenote:".</span><span class="sxs-lookup"><span data-stu-id="b1676-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="b1676-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1676-134">Response</span></span>

<span data-ttu-id="b1676-135">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [записной](../resources/notebook.md) книжки в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b1676-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1676-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b1676-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1676-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1676-137">Request</span></span>
<span data-ttu-id="b1676-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1676-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1676-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1676-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="c"></a>[<span data-ttu-id="b1676-140">C#</span><span class="sxs-lookup"><span data-stu-id="b1676-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1676-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1676-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1676-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1676-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b1676-143">Java</span><span class="sxs-lookup"><span data-stu-id="b1676-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-fromweburl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b1676-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1676-144">Response</span></span>
<span data-ttu-id="b1676-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1676-145">Here is an example of the response.</span></span> 

><span data-ttu-id="b1676-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b1676-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json; odata.metadata=minimal
Content-Length: 544

{
    "isDefault": true,
    "userRole": "userRole-value",
    "isShared": true,
    "sectionsUrl": "sectionUrl-value",
    "sectionGroupsUrl": "sectionGroupUrl-value",
    "links": {
        "oneNoteClientUrl": {
            "href": "href-value"
        },
        "oneNoteWebUrl": {
            "href": "href-value"
        }
    },
    "id": "id-value",
    "self": "self-value",
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


