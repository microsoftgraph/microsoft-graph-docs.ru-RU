---
title: Удаление Акцессревиев
description: В функции рецензирования Access Azure AD удалите объект Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d7a7434d4de008ce2a3f597636c30fcf014f3de8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258984"
---
# <a name="delete-accessreview"></a><span data-ttu-id="b0188-103">Удаление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="b0188-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0188-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD удалите объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="b0188-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0188-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0188-105">Permissions</span></span>
<span data-ttu-id="b0188-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0188-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0188-108">Permission type</span></span>                        | <span data-ttu-id="b0188-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0188-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0188-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0188-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0188-111">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0188-111">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b0188-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0188-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0188-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0188-113">Not supported.</span></span> |
|<span data-ttu-id="b0188-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0188-114">Application</span></span>                            | <span data-ttu-id="b0188-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0188-115">Not supported.</span></span> |

<span data-ttu-id="b0188-116">Вызывающая сторона также должна иметь разрешение Програмконтрол. ReadWrite. ALL, чтобы оно могло удалить [програмконтрол](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="b0188-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="b0188-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0188-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="b0188-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0188-118">Request headers</span></span>
| <span data-ttu-id="b0188-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b0188-119">Name</span></span>         | <span data-ttu-id="b0188-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b0188-120">Type</span></span>        | <span data-ttu-id="b0188-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b0188-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b0188-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0188-122">Authorization</span></span> | <span data-ttu-id="b0188-123">string</span><span class="sxs-lookup"><span data-stu-id="b0188-123">string</span></span> | <span data-ttu-id="b0188-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0188-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0188-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0188-126">Request body</span></span>
<span data-ttu-id="b0188-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0188-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b0188-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0188-128">Response</span></span>
<span data-ttu-id="b0188-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b0188-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0188-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b0188-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0188-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0188-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
##### <a name="response"></a><span data-ttu-id="b0188-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0188-133">Response</span></span>
><span data-ttu-id="b0188-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0188-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b0188-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b0188-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b0188-137">C#</span><span class="sxs-lookup"><span data-stu-id="b0188-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0188-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0188-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_accessReview-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b0188-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0188-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_accessReview-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
