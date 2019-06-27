---
title: Удаление educationAssignment
description: Удаление существующего назначения. Удалять назначения могут только преподаватели внутри класса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 408e5495a816de2832a3ac18d40110cd79c1b979
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259943"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="e5891-104">Удаление educationAssignment</span><span class="sxs-lookup"><span data-stu-id="e5891-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5891-105">Удаление существующего назначения.</span><span class="sxs-lookup"><span data-stu-id="e5891-105">Delete an existing assignment.</span></span> <span data-ttu-id="e5891-106">Удалять назначения могут только преподаватели внутри класса.</span><span class="sxs-lookup"><span data-stu-id="e5891-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5891-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5891-107">Permissions</span></span>

<span data-ttu-id="e5891-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5891-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5891-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5891-110">Permission type</span></span>                        | <span data-ttu-id="e5891-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5891-111">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="e5891-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5891-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5891-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5891-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="e5891-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5891-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5891-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5891-115">Not Supported.</span></span>                                          |
| <span data-ttu-id="e5891-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5891-116">Application</span></span>                            | <span data-ttu-id="e5891-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5891-117">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="e5891-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5891-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e5891-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5891-119">Request headers</span></span>

| <span data-ttu-id="e5891-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5891-120">Header</span></span>        | <span data-ttu-id="e5891-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5891-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e5891-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5891-122">Authorization</span></span> | <span data-ttu-id="e5891-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5891-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5891-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5891-125">Request body</span></span>

<span data-ttu-id="e5891-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5891-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5891-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5891-127">Response</span></span>

<span data-ttu-id="e5891-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e5891-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5891-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e5891-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5891-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5891-131">Request</span></span>

<span data-ttu-id="e5891-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5891-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="e5891-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5891-133">Response</span></span>
<span data-ttu-id="e5891-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5891-134">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e5891-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e5891-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e5891-136">C#</span><span class="sxs-lookup"><span data-stu-id="e5891-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5891-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="e5891-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e5891-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e5891-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_educationassignment-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
