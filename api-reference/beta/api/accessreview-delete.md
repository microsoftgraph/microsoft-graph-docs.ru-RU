---
title: Удаление Акцессревиев
description: В функции рецензирования Access Azure AD удалите объект Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: daf96b917c8c285f06f803179c4c1eff5b913f86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441937"
---
# <a name="delete-accessreview"></a><span data-ttu-id="a2032-103">Удаление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="a2032-103">Delete accessReview</span></span>

<span data-ttu-id="a2032-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a2032-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2032-105">В функции [рецензирования Access](../resources/accessreviews-root.md) Azure AD удалите объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="a2032-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a2032-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2032-106">Permissions</span></span>
<span data-ttu-id="a2032-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2032-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2032-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2032-109">Permission type</span></span>                        | <span data-ttu-id="a2032-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2032-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2032-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2032-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2032-112">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a2032-112">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a2032-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2032-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2032-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2032-114">Not supported.</span></span> |
|<span data-ttu-id="a2032-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2032-115">Application</span></span>                            | <span data-ttu-id="a2032-116">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="a2032-116">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="a2032-117">Вызывающая сторона также должна иметь разрешение Програмконтрол. ReadWrite. ALL, чтобы оно могло удалить [програмконтрол](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="a2032-117">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="a2032-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2032-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="a2032-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2032-119">Request headers</span></span>
| <span data-ttu-id="a2032-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a2032-120">Name</span></span>         | <span data-ttu-id="a2032-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a2032-121">Type</span></span>        | <span data-ttu-id="a2032-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a2032-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a2032-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2032-123">Authorization</span></span> | <span data-ttu-id="a2032-124">string</span><span class="sxs-lookup"><span data-stu-id="a2032-124">string</span></span> | <span data-ttu-id="a2032-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2032-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2032-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2032-127">Request body</span></span>
<span data-ttu-id="a2032-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2032-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a2032-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2032-129">Response</span></span>
<span data-ttu-id="a2032-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a2032-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2032-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a2032-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a2032-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2032-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a2032-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2032-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="c"></a>[<span data-ttu-id="a2032-135">C#</span><span class="sxs-lookup"><span data-stu-id="a2032-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2032-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2032-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2032-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2032-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a2032-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2032-138">Response</span></span>
><span data-ttu-id="a2032-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2032-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
