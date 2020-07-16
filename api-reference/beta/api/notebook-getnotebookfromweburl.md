---
title: 'Записная книжка: Жетнотебукфромвебурл'
description: Получение свойств и связей объекта записной книжки с помощью URL-пути.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 6b42bd6425b35333f7f14021182bc4141497e1a1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44894825"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="b23bc-103">Записная книжка: Жетнотебукфромвебурл</span><span class="sxs-lookup"><span data-stu-id="b23bc-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="b23bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b23bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b23bc-105">Получение свойств и связей объекта [записной книжки](../resources/notebook.md) с помощью URL-пути.</span><span class="sxs-lookup"><span data-stu-id="b23bc-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="b23bc-106">Местоположение может представлять собой записные книжки пользователя Microsoft 365, групповые записные книжки или размещенные на сайтах SharePoint записные книжки группы в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b23bc-106">The location can be user notebooks on Microsoft 365, group notebooks, or SharePoint site-hosted team notebooks on Microsoft 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="b23bc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b23bc-107">Permissions</span></span>
<span data-ttu-id="b23bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b23bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b23bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b23bc-110">Permission type</span></span>      | <span data-ttu-id="b23bc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b23bc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b23bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b23bc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b23bc-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23bc-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b23bc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b23bc-114">Application</span></span> | <span data-ttu-id="b23bc-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23bc-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b23bc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b23bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="b23bc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b23bc-117">Request headers</span></span>
| <span data-ttu-id="b23bc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b23bc-118">Name</span></span>       | <span data-ttu-id="b23bc-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b23bc-119">Type</span></span> | <span data-ttu-id="b23bc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b23bc-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b23bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b23bc-121">Authorization</span></span>  | <span data-ttu-id="b23bc-122">string</span><span class="sxs-lookup"><span data-stu-id="b23bc-122">string</span></span>  | <span data-ttu-id="b23bc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b23bc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b23bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b23bc-125">Accept</span></span> | <span data-ttu-id="b23bc-126">строка</span><span class="sxs-lookup"><span data-stu-id="b23bc-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b23bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b23bc-127">Request body</span></span>
<span data-ttu-id="b23bc-128">В тексте запроса добавьте представление в формате JSON полного URL-пути к записной книжке, которую необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="b23bc-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="b23bc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b23bc-129">Property</span></span>     | <span data-ttu-id="b23bc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b23bc-130">Type</span></span>        | <span data-ttu-id="b23bc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b23bc-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="b23bc-132">Путь URL-адреса извлекаемой записной книжки.</span><span class="sxs-lookup"><span data-stu-id="b23bc-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="b23bc-133">Он также может содержать префикс "OneNote:".</span><span class="sxs-lookup"><span data-stu-id="b23bc-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="b23bc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b23bc-134">Response</span></span>

<span data-ttu-id="b23bc-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b23bc-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b23bc-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b23bc-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b23bc-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b23bc-137">Request</span></span>
<span data-ttu-id="b23bc-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b23bc-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b23bc-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b23bc-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
# <a name="c"></a>[<span data-ttu-id="b23bc-140">C#</span><span class="sxs-lookup"><span data-stu-id="b23bc-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/notebook-fromweburl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b23bc-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b23bc-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/notebook-fromweburl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b23bc-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b23bc-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/notebook-fromweburl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b23bc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b23bc-143">Response</span></span>
<span data-ttu-id="b23bc-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b23bc-144">Here is an example of the response.</span></span> 

><span data-ttu-id="b23bc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b23bc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
