---
title: 'Привилежедаппровал: Мирекуестс'
description: Получение запросов утверждения запрашивающей стороны.
localization_priority: Normal
ms.openlocfilehash: 71c9ffd79a48df0e4c9bc9fa84c9f61dca1a0594
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267727"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="82358-103">Привилежедаппровал: Мирекуестс</span><span class="sxs-lookup"><span data-stu-id="82358-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82358-104">Получение запросов утверждения запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="82358-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="82358-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82358-105">Permissions</span></span>
<span data-ttu-id="82358-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="82358-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82358-108">Permission type</span></span>      | <span data-ttu-id="82358-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82358-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82358-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82358-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82358-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="82358-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82358-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82358-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82358-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82358-113">Not supported.</span></span>    |
|<span data-ttu-id="82358-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82358-114">Application</span></span> | <span data-ttu-id="82358-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82358-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82358-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82358-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="82358-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82358-117">Request headers</span></span>
| <span data-ttu-id="82358-118">Имя</span><span class="sxs-lookup"><span data-stu-id="82358-118">Name</span></span>       | <span data-ttu-id="82358-119">Описание</span><span class="sxs-lookup"><span data-stu-id="82358-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="82358-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82358-120">Authorization</span></span>  | <span data-ttu-id="82358-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82358-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82358-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82358-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="82358-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="82358-124">Response</span></span>

<span data-ttu-id="82358-125">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82358-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="82358-126">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="82358-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="82358-127">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="82358-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="82358-128">Пример</span><span class="sxs-lookup"><span data-stu-id="82358-128">Example</span></span>
<span data-ttu-id="82358-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="82358-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="82358-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="82358-130">Request</span></span>
<span data-ttu-id="82358-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82358-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="82358-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="82358-132">Response</span></span>
<span data-ttu-id="82358-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82358-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="82358-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="82358-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="82358-137">C#</span><span class="sxs-lookup"><span data-stu-id="82358-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedapproval_myrequests-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82358-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="82358-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedapproval_myrequests-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="82358-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82358-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/privilegedapproval_myrequests-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-myrequests.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
