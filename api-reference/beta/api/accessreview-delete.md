---
title: Удаление Акцессревиев
description: В функции рецензирования Access Azure AD удалите объект Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adc47fbbee90330af210207470afc25fb859d970
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049605"
---
# <a name="delete-accessreview"></a><span data-ttu-id="abe43-103">Удаление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="abe43-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe43-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD удалите объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="abe43-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="abe43-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abe43-105">Permissions</span></span>
<span data-ttu-id="abe43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abe43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abe43-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abe43-108">Permission type</span></span>                        | <span data-ttu-id="abe43-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abe43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="abe43-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abe43-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="abe43-111">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abe43-111">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="abe43-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abe43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abe43-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abe43-113">Not supported.</span></span> |
|<span data-ttu-id="abe43-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abe43-114">Application</span></span>                            | <span data-ttu-id="abe43-115">Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="abe43-115">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="abe43-116">Вызывающая сторона также должна иметь разрешение Програмконтрол. ReadWrite. ALL, чтобы оно могло удалить [програмконтрол](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="abe43-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="abe43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abe43-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="abe43-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abe43-118">Request headers</span></span>
| <span data-ttu-id="abe43-119">Имя</span><span class="sxs-lookup"><span data-stu-id="abe43-119">Name</span></span>         | <span data-ttu-id="abe43-120">Тип</span><span class="sxs-lookup"><span data-stu-id="abe43-120">Type</span></span>        | <span data-ttu-id="abe43-121">Описание</span><span class="sxs-lookup"><span data-stu-id="abe43-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="abe43-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="abe43-122">Authorization</span></span> | <span data-ttu-id="abe43-123">string</span><span class="sxs-lookup"><span data-stu-id="abe43-123">string</span></span> | <span data-ttu-id="abe43-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abe43-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="abe43-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="abe43-126">Request body</span></span>
<span data-ttu-id="abe43-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abe43-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="abe43-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="abe43-128">Response</span></span>
<span data-ttu-id="abe43-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="abe43-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abe43-131">Пример</span><span class="sxs-lookup"><span data-stu-id="abe43-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abe43-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="abe43-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="abe43-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="abe43-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="abe43-134">C#</span><span class="sxs-lookup"><span data-stu-id="abe43-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="abe43-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="abe43-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="abe43-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="abe43-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="abe43-137">Java</span><span class="sxs-lookup"><span data-stu-id="abe43-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="abe43-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="abe43-138">Response</span></span>
><span data-ttu-id="abe43-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abe43-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
