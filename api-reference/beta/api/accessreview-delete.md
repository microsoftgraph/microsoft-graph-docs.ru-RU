---
title: Удаление Акцессревиев
description: В функции рецензирования Access Azure AD удалите объект Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0795ef56c395c0eb9bf8b65f4a941d23b3ee5472
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408864"
---
# <a name="delete-accessreview"></a><span data-ttu-id="8f2d7-103">Удаление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="8f2d7-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f2d7-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD удалите объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="8f2d7-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f2d7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f2d7-105">Permissions</span></span>
<span data-ttu-id="8f2d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f2d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f2d7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f2d7-108">Permission type</span></span>                        | <span data-ttu-id="8f2d7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f2d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f2d7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f2d7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f2d7-111">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8f2d7-111">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="8f2d7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f2d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f2d7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f2d7-113">Not supported.</span></span> |
|<span data-ttu-id="8f2d7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f2d7-114">Application</span></span>                            | <span data-ttu-id="8f2d7-115">Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="8f2d7-115">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="8f2d7-116">Вызывающая сторона также должна иметь разрешение Програмконтрол. ReadWrite. ALL, чтобы оно могло удалить [програмконтрол](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="8f2d7-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="8f2d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f2d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="8f2d7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f2d7-118">Request headers</span></span>
| <span data-ttu-id="8f2d7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f2d7-119">Name</span></span>         | <span data-ttu-id="8f2d7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8f2d7-120">Type</span></span>        | <span data-ttu-id="8f2d7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8f2d7-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8f2d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f2d7-122">Authorization</span></span> | <span data-ttu-id="8f2d7-123">string</span><span class="sxs-lookup"><span data-stu-id="8f2d7-123">string</span></span> | <span data-ttu-id="8f2d7-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f2d7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f2d7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f2d7-126">Request body</span></span>
<span data-ttu-id="8f2d7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f2d7-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8f2d7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f2d7-128">Response</span></span>
<span data-ttu-id="8f2d7-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8f2d7-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f2d7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8f2d7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f2d7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f2d7-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f2d7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f2d7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f2d7-134">C#</span><span class="sxs-lookup"><span data-stu-id="8f2d7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f2d7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f2d7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f2d7-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f2d7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8f2d7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f2d7-137">Response</span></span>
><span data-ttu-id="8f2d7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f2d7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
