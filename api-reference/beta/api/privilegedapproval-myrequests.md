---
title: 'Привилежедаппровал: Мирекуестс'
description: Получение запросов утверждения запрашивающей стороны.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f03ac0665723c9802dc9d460c5997023c4d42287
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723471"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="ab82d-103">Привилежедаппровал: Мирекуестс</span><span class="sxs-lookup"><span data-stu-id="ab82d-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab82d-104">Получение запросов утверждения запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="ab82d-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab82d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab82d-105">Permissions</span></span>
<span data-ttu-id="ab82d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab82d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ab82d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab82d-108">Permission type</span></span>      | <span data-ttu-id="ab82d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab82d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab82d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab82d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab82d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab82d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab82d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab82d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab82d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab82d-113">Not supported.</span></span>    |
|<span data-ttu-id="ab82d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab82d-114">Application</span></span> | <span data-ttu-id="ab82d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab82d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab82d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab82d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="ab82d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab82d-117">Request headers</span></span>
| <span data-ttu-id="ab82d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ab82d-118">Name</span></span>       | <span data-ttu-id="ab82d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ab82d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab82d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab82d-120">Authorization</span></span>  | <span data-ttu-id="ab82d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab82d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab82d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab82d-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ab82d-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab82d-124">Response</span></span>

<span data-ttu-id="ab82d-125">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab82d-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="ab82d-126">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="ab82d-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ab82d-127">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="ab82d-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="ab82d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ab82d-128">Example</span></span>
<span data-ttu-id="ab82d-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ab82d-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab82d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab82d-130">Request</span></span>
<span data-ttu-id="ab82d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab82d-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ab82d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab82d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ab82d-133">C#</span><span class="sxs-lookup"><span data-stu-id="ab82d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedapproval-myrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab82d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab82d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedapproval-myrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ab82d-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ab82d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedapproval-myrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ab82d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab82d-136">Response</span></span>
<span data-ttu-id="ab82d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab82d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
