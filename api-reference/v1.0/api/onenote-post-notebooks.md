---
title: Создание записной книжки
description: Создайте новую записную книжку OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: b7194458e1bac49079da623400eb932979491358
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611780"
---
# <a name="create-notebook"></a><span data-ttu-id="228bb-103">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="228bb-103">Create notebook</span></span>

<span data-ttu-id="228bb-104">Создайте новую записную [книжку](../resources/notebook.md)OneNote.</span><span class="sxs-lookup"><span data-stu-id="228bb-104">Create a new OneNote [notebook](../resources/notebook.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="228bb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="228bb-105">Permissions</span></span>
<span data-ttu-id="228bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="228bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="228bb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="228bb-108">Permission type</span></span>      | <span data-ttu-id="228bb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="228bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="228bb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="228bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="228bb-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228bb-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="228bb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="228bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="228bb-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228bb-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="228bb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="228bb-114">Application</span></span> | <span data-ttu-id="228bb-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228bb-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="228bb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="228bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks
POST /users/{id | userPrincipalName}/onenote/notebooks
POST /groups/{id}/onenote/notebooks
POST /sites/{id}/onenote/notebooks
```
## <a name="request-headers"></a><span data-ttu-id="228bb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="228bb-117">Request headers</span></span>
| <span data-ttu-id="228bb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="228bb-118">Name</span></span>       | <span data-ttu-id="228bb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="228bb-119">Type</span></span> | <span data-ttu-id="228bb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="228bb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="228bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="228bb-121">Authorization</span></span>  | <span data-ttu-id="228bb-122">string</span><span class="sxs-lookup"><span data-stu-id="228bb-122">string</span></span>  | <span data-ttu-id="228bb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="228bb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="228bb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="228bb-125">Content-Type</span></span> | <span data-ttu-id="228bb-126">string</span><span class="sxs-lookup"><span data-stu-id="228bb-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="228bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="228bb-127">Request body</span></span>
<span data-ttu-id="228bb-128">В тексте запроса укажите имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="228bb-128">In the request body, supply a name for the notebook.</span></span> 

<span data-ttu-id="228bb-129">Имена записных книжек должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="228bb-129">Notebook names must be unique.</span></span> <span data-ttu-id="228bb-130">Имя не может содержать более 128 символов или содержать следующие символы: _Км_ \*\/: _лт__гт_ | ' "</span><span class="sxs-lookup"><span data-stu-id="228bb-130">The name cannot contain more than 128 characters or contain the following characters:  ?\*\/:<>|'"</span></span>

## <a name="response"></a><span data-ttu-id="228bb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="228bb-131">Response</span></span>

<span data-ttu-id="228bb-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [записной книжки](../resources/notebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="228bb-132">If successful, this method returns a `201 Created` response code and the new [notebook](../resources/notebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="228bb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="228bb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="228bb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="228bb-134">Request</span></span>
<span data-ttu-id="228bb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="228bb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_notebook_from_onenote"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks
Content-type: application/json
Content-length: 30

{
  "displayName": "Notebook name"
}
```

##### <a name="response"></a><span data-ttu-id="228bb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="228bb-136">Response</span></span>
<span data-ttu-id="228bb-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="228bb-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 284

{
  "isDefault": true,
  "userRole": {
  },
  "isShared": true,
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="228bb-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="228bb-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="228bb-141">Языках</span><span class="sxs-lookup"><span data-stu-id="228bb-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_notebook_from_onenote-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="228bb-142">Язык</span><span class="sxs-lookup"><span data-stu-id="228bb-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_notebook_from_onenote-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/onenote-post-notebooks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/onenote-post-notebooks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
