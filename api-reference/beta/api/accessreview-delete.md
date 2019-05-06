---
title: Удаление Акцессревиев
description: В функции рецензирования Access Azure AD удалите объект Акцессревиев.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7291f334b08225f599833fe3a7351a4276d1399a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586306"
---
# <a name="delete-accessreview"></a><span data-ttu-id="353ce-103">Удаление Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="353ce-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="353ce-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD удалите объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="353ce-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="353ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="353ce-105">Permissions</span></span>
<span data-ttu-id="353ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="353ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="353ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="353ce-108">Permission type</span></span>                        | <span data-ttu-id="353ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="353ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="353ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="353ce-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="353ce-111">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="353ce-111">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="353ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="353ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="353ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="353ce-113">Not supported.</span></span> |
|<span data-ttu-id="353ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="353ce-114">Application</span></span>                            | <span data-ttu-id="353ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="353ce-115">Not supported.</span></span> |

<span data-ttu-id="353ce-116">Вызывающая сторона также должна иметь разрешение Програмконтрол. ReadWrite. ALL, чтобы оно могло удалить [програмконтрол](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="353ce-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="353ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="353ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="353ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="353ce-118">Request headers</span></span>
| <span data-ttu-id="353ce-119">Имя</span><span class="sxs-lookup"><span data-stu-id="353ce-119">Name</span></span>         | <span data-ttu-id="353ce-120">Тип</span><span class="sxs-lookup"><span data-stu-id="353ce-120">Type</span></span>        | <span data-ttu-id="353ce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="353ce-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="353ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="353ce-122">Authorization</span></span> | <span data-ttu-id="353ce-123">string</span><span class="sxs-lookup"><span data-stu-id="353ce-123">string</span></span> | <span data-ttu-id="353ce-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="353ce-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="353ce-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="353ce-126">Request body</span></span>
<span data-ttu-id="353ce-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="353ce-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="353ce-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="353ce-128">Response</span></span>
<span data-ttu-id="353ce-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="353ce-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="353ce-131">Пример</span><span class="sxs-lookup"><span data-stu-id="353ce-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="353ce-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="353ce-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
##### <a name="response"></a><span data-ttu-id="353ce-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="353ce-133">Response</span></span>
><span data-ttu-id="353ce-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="353ce-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="353ce-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="353ce-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="353ce-137">Языках</span><span class="sxs-lookup"><span data-stu-id="353ce-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="353ce-138">Язык</span><span class="sxs-lookup"><span data-stu-id="353ce-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_accessReview-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
