---
title: 'Записная книжка: Жетнотебукфромвебурл'
description: Получение свойств и связей объекта записной книжки с помощью URL-пути.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: dedaa2937e3f98333c3cae83652d0e448698492f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374478"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="23a3c-103">Записная книжка: Жетнотебукфромвебурл</span><span class="sxs-lookup"><span data-stu-id="23a3c-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="23a3c-104">Получение свойств и связей объекта записной [книжки](../resources/notebook.md) с помощью URL-пути.</span><span class="sxs-lookup"><span data-stu-id="23a3c-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="23a3c-105">Местоположение может представлять собой записные книжки для пользователей в Office 365, групповые записные книжки или записные книжки группы, размещаемые в SharePoint, в Office 365.</span><span class="sxs-lookup"><span data-stu-id="23a3c-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="23a3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23a3c-106">Permissions</span></span>
<span data-ttu-id="23a3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23a3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23a3c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23a3c-109">Permission type</span></span>      | <span data-ttu-id="23a3c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23a3c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23a3c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23a3c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="23a3c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23a3c-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="23a3c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23a3c-113">Application</span></span> | <span data-ttu-id="23a3c-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23a3c-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23a3c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23a3c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="23a3c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23a3c-116">Request headers</span></span>
| <span data-ttu-id="23a3c-117">Имя</span><span class="sxs-lookup"><span data-stu-id="23a3c-117">Name</span></span>       | <span data-ttu-id="23a3c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="23a3c-118">Type</span></span> | <span data-ttu-id="23a3c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="23a3c-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23a3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="23a3c-120">Authorization</span></span>  | <span data-ttu-id="23a3c-121">string</span><span class="sxs-lookup"><span data-stu-id="23a3c-121">string</span></span>  | <span data-ttu-id="23a3c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23a3c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="23a3c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="23a3c-124">Accept</span></span> | <span data-ttu-id="23a3c-125">строка</span><span class="sxs-lookup"><span data-stu-id="23a3c-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="23a3c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23a3c-126">Request body</span></span>
<span data-ttu-id="23a3c-127">В тексте запроса добавьте представление в формате JSON полного URL-пути к записной книжке, которую необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="23a3c-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="23a3c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="23a3c-128">Property</span></span>     | <span data-ttu-id="23a3c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="23a3c-129">Type</span></span>        | <span data-ttu-id="23a3c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="23a3c-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="23a3c-131">Путь URL-адреса извлекаемой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="23a3c-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="23a3c-132">Он также может содержать префикс "OneNote:".</span><span class="sxs-lookup"><span data-stu-id="23a3c-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="23a3c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="23a3c-133">Response</span></span>

<span data-ttu-id="23a3c-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="23a3c-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23a3c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="23a3c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23a3c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="23a3c-136">Request</span></span>
<span data-ttu-id="23a3c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23a3c-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="23a3c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="23a3c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23a3c-139">C#</span><span class="sxs-lookup"><span data-stu-id="23a3c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23a3c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23a3c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23a3c-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="23a3c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23a3c-142">Java</span><span class="sxs-lookup"><span data-stu-id="23a3c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/notebook-fromweburl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="23a3c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="23a3c-143">Response</span></span>
<span data-ttu-id="23a3c-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23a3c-144">Here is an example of the response.</span></span> 

><span data-ttu-id="23a3c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23a3c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
