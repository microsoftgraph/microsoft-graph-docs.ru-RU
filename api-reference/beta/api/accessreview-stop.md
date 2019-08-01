---
title: Остановить Акцессревиев
description: В функции рецензирования Access Azure AD остановите текущую активную Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  (Чтобы не допустить запуск последующих экземпляров проверки доступа, обновите его, чтобы изменить запланированную дату окончания).  После остановки проверки доступа рецензенты больше не могут вводить входные данные, а решения проверки доступа могут быть применены.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6e5efce41b4f45fa48e0c9c247a6886ff555e94c
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049574"
---
# <a name="stop-accessreview"></a><span data-ttu-id="39183-106">Остановить Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="39183-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39183-107">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD остановите текущую активную [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="39183-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="39183-108">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="39183-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="39183-109">(Чтобы не допустить запуск последующих экземпляров проверки доступа, обновите [его](accessreview-update.md) , чтобы изменить запланированную дату окончания).</span><span class="sxs-lookup"><span data-stu-id="39183-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="39183-110">После остановки проверки доступа рецензенты больше не могут вводить входные данные, а решения проверки доступа могут быть применены.</span><span class="sxs-lookup"><span data-stu-id="39183-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="39183-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39183-111">Permissions</span></span>
<span data-ttu-id="39183-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39183-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39183-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39183-114">Permission type</span></span>                        | <span data-ttu-id="39183-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39183-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="39183-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39183-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="39183-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39183-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="39183-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39183-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39183-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39183-119">Not supported.</span></span> |
|<span data-ttu-id="39183-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39183-120">Application</span></span>                            | <span data-ttu-id="39183-121">Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="39183-121">AccessReview.ReadWrite.Membership</span></span>  |

## <a name="http-request"></a><span data-ttu-id="39183-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39183-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="39183-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39183-123">Request headers</span></span>
| <span data-ttu-id="39183-124">Имя</span><span class="sxs-lookup"><span data-stu-id="39183-124">Name</span></span>         | <span data-ttu-id="39183-125">Тип</span><span class="sxs-lookup"><span data-stu-id="39183-125">Type</span></span>        | <span data-ttu-id="39183-126">Описание</span><span class="sxs-lookup"><span data-stu-id="39183-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="39183-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="39183-127">Authorization</span></span> | <span data-ttu-id="39183-128">string</span><span class="sxs-lookup"><span data-stu-id="39183-128">string</span></span> | <span data-ttu-id="39183-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39183-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39183-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39183-131">Request body</span></span>
<span data-ttu-id="39183-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39183-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="39183-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="39183-133">Response</span></span>
<span data-ttu-id="39183-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="39183-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39183-136">Пример</span><span class="sxs-lookup"><span data-stu-id="39183-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39183-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="39183-137">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="39183-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="39183-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="39183-139">C#</span><span class="sxs-lookup"><span data-stu-id="39183-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39183-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="39183-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="39183-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="39183-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="39183-142">Java</span><span class="sxs-lookup"><span data-stu-id="39183-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="39183-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="39183-143">Response</span></span>
><span data-ttu-id="39183-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39183-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
