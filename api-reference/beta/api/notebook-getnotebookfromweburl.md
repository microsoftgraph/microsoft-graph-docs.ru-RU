---
title: 'Записная книжка: Жетнотебукфромвебурл'
description: Получение свойств и связей объекта записной книжки с помощью URL-пути.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d81454144cfaa62c9641fc6a524bbd752f6ee30d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450389"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="a8650-103">Записная книжка: Жетнотебукфромвебурл</span><span class="sxs-lookup"><span data-stu-id="a8650-103">notebook: getNotebookFromWebUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8650-104">Получение свойств и связей объекта записной [книжки](../resources/notebook.md) с помощью URL-пути.</span><span class="sxs-lookup"><span data-stu-id="a8650-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="a8650-105">Местоположение может представлять собой записные книжки для пользователей в Office 365, групповые записные книжки или записные книжки группы, размещаемые в SharePoint, в Office 365.</span><span class="sxs-lookup"><span data-stu-id="a8650-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8650-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8650-106">Permissions</span></span>
<span data-ttu-id="a8650-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8650-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8650-109">Permission type</span></span>      | <span data-ttu-id="a8650-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8650-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8650-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8650-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a8650-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8650-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a8650-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8650-113">Application</span></span> | <span data-ttu-id="a8650-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8650-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8650-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8650-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="a8650-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8650-116">Request headers</span></span>
| <span data-ttu-id="a8650-117">Имя</span><span class="sxs-lookup"><span data-stu-id="a8650-117">Name</span></span>       | <span data-ttu-id="a8650-118">Тип</span><span class="sxs-lookup"><span data-stu-id="a8650-118">Type</span></span> | <span data-ttu-id="a8650-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a8650-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a8650-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8650-120">Authorization</span></span>  | <span data-ttu-id="a8650-121">string</span><span class="sxs-lookup"><span data-stu-id="a8650-121">string</span></span>  | <span data-ttu-id="a8650-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8650-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8650-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a8650-124">Accept</span></span> | <span data-ttu-id="a8650-125">строка</span><span class="sxs-lookup"><span data-stu-id="a8650-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a8650-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8650-126">Request body</span></span>
<span data-ttu-id="a8650-127">В тексте запроса добавьте представление в формате JSON полного URL-пути к записной книжке, которую необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="a8650-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="a8650-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8650-128">Property</span></span>     | <span data-ttu-id="a8650-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a8650-129">Type</span></span>        | <span data-ttu-id="a8650-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a8650-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="a8650-131">Путь URL-адреса извлекаемой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="a8650-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="a8650-132">Он также может содержать префикс "OneNote:".</span><span class="sxs-lookup"><span data-stu-id="a8650-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="a8650-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8650-133">Response</span></span>

<span data-ttu-id="a8650-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8650-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8650-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a8650-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8650-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8650-136">Request</span></span>
<span data-ttu-id="a8650-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8650-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8650-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8650-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8650-139">C#</span><span class="sxs-lookup"><span data-stu-id="a8650-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8650-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8650-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8650-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a8650-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a8650-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8650-142">Response</span></span>
<span data-ttu-id="a8650-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8650-143">Here is an example of the response.</span></span> 

><span data-ttu-id="a8650-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8650-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
