---
title: 'notebook: getRecentNotebooks'
description: Получите список экземпляров recentNotebook, которые недавно открывал вошедший в систему пользователь.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: ed5788c9d53baa0dc0f46de12dda615a0a783dd6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274545"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="797c6-103">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="797c6-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="797c6-104">Получите список экземпляров [recentNotebook](../resources/recentnotebook.md), которые недавно открывал вошедший в систему пользователь.</span><span class="sxs-lookup"><span data-stu-id="797c6-104">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="797c6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="797c6-105">Permissions</span></span>
<span data-ttu-id="797c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="797c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="797c6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="797c6-108">Permission type</span></span>      | <span data-ttu-id="797c6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="797c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="797c6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="797c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="797c6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="797c6-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="797c6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="797c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="797c6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="797c6-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="797c6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="797c6-114">Application</span></span> | <span data-ttu-id="797c6-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="797c6-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="797c6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="797c6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="797c6-117">Идентификатор `{id | userPrincipalName}` должен соответствовать пользователю, закодированному в токене авторизации, используемом для выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="797c6-117">The `{id | userPrincipalName}` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="797c6-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="797c6-118">Function parameters</span></span>

| <span data-ttu-id="797c6-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="797c6-119">Parameter</span></span>    | <span data-ttu-id="797c6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="797c6-120">Type</span></span>   |<span data-ttu-id="797c6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="797c6-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="797c6-122">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="797c6-122">includePersonalNotebooks</span></span>|<span data-ttu-id="797c6-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="797c6-123">Boolean</span></span>|<span data-ttu-id="797c6-124">Включите записные книжки, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="797c6-124">Include notebooks owned by the user.</span></span> <span data-ttu-id="797c6-125">Установите значение `true`, чтобы включить записные книжки, принадлежащие пользователю; в противном случае установите значение `false`.</span><span class="sxs-lookup"><span data-stu-id="797c6-125">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="797c6-126">Если вы не включите параметр `includePersonalNotebooks`, запрос вернет ошибку `400`.</span><span class="sxs-lookup"><span data-stu-id="797c6-126">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="797c6-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="797c6-127">Request headers</span></span>
| <span data-ttu-id="797c6-128">Имя</span><span class="sxs-lookup"><span data-stu-id="797c6-128">Name</span></span>       | <span data-ttu-id="797c6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="797c6-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="797c6-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="797c6-130">Authorization</span></span>  | <span data-ttu-id="797c6-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="797c6-131">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="797c6-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="797c6-132">Request body</span></span>
<span data-ttu-id="797c6-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="797c6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="797c6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="797c6-134">Response</span></span>
<span data-ttu-id="797c6-135">В случае успеха возвращается ответ с кодом `200 OK`, который содержит JSON-коллекцию ресурсов **recentNotebook**.</span><span class="sxs-lookup"><span data-stu-id="797c6-135">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="797c6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="797c6-136">Example</span></span>
<span data-ttu-id="797c6-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="797c6-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="797c6-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="797c6-138">Request</span></span>
<span data-ttu-id="797c6-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="797c6-139">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="797c6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="797c6-140">Response</span></span>
<span data-ttu-id="797c6-141">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="797c6-141">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="797c6-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="797c6-142">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="797c6-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="797c6-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/recent_notebooks-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="797c6-144">C#</span><span class="sxs-lookup"><span data-stu-id="797c6-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/recent_notebooks-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="797c6-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="797c6-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/recent_notebooks-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/notebook-getrecentnotebooks.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/notebook-getrecentnotebooks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/notebook-getrecentnotebooks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
