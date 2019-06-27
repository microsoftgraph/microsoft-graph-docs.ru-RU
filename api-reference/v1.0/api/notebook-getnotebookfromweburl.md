---
title: 'Записная книжка: Жетнотебукфромвебурл'
description: Получение свойств и связей объекта записной книжки с помощью URL-пути.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 07de07b1771fd74f2b2c2dc1e3b9a3dc5276fa80
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274573"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="ced3a-103">Записная книжка: Жетнотебукфромвебурл</span><span class="sxs-lookup"><span data-stu-id="ced3a-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="ced3a-104">Получение свойств и связей объекта записной [книжки](../resources/notebook.md) с помощью URL-пути.</span><span class="sxs-lookup"><span data-stu-id="ced3a-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="ced3a-105">Местоположение может представлять собой записные книжки для пользователей в Office 365, групповые записные книжки или записные книжки группы, размещаемые в SharePoint, в Office 365.</span><span class="sxs-lookup"><span data-stu-id="ced3a-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="ced3a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ced3a-106">Permissions</span></span>
<span data-ttu-id="ced3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ced3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ced3a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ced3a-109">Permission type</span></span>      | <span data-ttu-id="ced3a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ced3a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ced3a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ced3a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ced3a-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced3a-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ced3a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ced3a-113">Application</span></span> | <span data-ttu-id="ced3a-114">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced3a-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ced3a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ced3a-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="ced3a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ced3a-116">Request headers</span></span>
| <span data-ttu-id="ced3a-117">Имя</span><span class="sxs-lookup"><span data-stu-id="ced3a-117">Name</span></span>       | <span data-ttu-id="ced3a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ced3a-118">Type</span></span> | <span data-ttu-id="ced3a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ced3a-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ced3a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ced3a-120">Authorization</span></span>  | <span data-ttu-id="ced3a-121">string</span><span class="sxs-lookup"><span data-stu-id="ced3a-121">string</span></span>  | <span data-ttu-id="ced3a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ced3a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ced3a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ced3a-124">Accept</span></span> | <span data-ttu-id="ced3a-125">строка</span><span class="sxs-lookup"><span data-stu-id="ced3a-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ced3a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ced3a-126">Request body</span></span>
<span data-ttu-id="ced3a-127">В тексте запроса добавьте представление в формате JSON полного URL-пути к записной книжке, которую необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="ced3a-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="ced3a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ced3a-128">Property</span></span>     | <span data-ttu-id="ced3a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ced3a-129">Type</span></span>        | <span data-ttu-id="ced3a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ced3a-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="ced3a-131">Путь URL-адреса извлекаемой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="ced3a-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="ced3a-132">Он также может содержать префикс "OneNote:".</span><span class="sxs-lookup"><span data-stu-id="ced3a-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="ced3a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ced3a-133">Response</span></span>

<span data-ttu-id="ced3a-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ced3a-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ced3a-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ced3a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ced3a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ced3a-136">Request</span></span>
<span data-ttu-id="ced3a-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ced3a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="ced3a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ced3a-138">Response</span></span>
<span data-ttu-id="ced3a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ced3a-139">Here is an example of the response.</span></span> 

><span data-ttu-id="ced3a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ced3a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ced3a-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ced3a-142">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ced3a-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="ced3a-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/notebook_fromweburl-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="ced3a-144">C#</span><span class="sxs-lookup"><span data-stu-id="ced3a-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/notebook_fromweburl-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ced3a-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ced3a-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/notebook_fromweburl-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/notebook-getnotebookfromweburl.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/notebook-getnotebookfromweburl.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-getnotebookfromweburl.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
