---
title: 'Привилежедаппровал: Мирекуестс'
description: Получение запросов утверждения запрашивающей стороны.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 8be41edff2c2c9163f26238ef0dd23bb61ea5170
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218803"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="2ba1c-103">Привилежедаппровал: Мирекуестс</span><span class="sxs-lookup"><span data-stu-id="2ba1c-103">privilegedApproval: myRequests</span></span>

<span data-ttu-id="2ba1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba1c-105">Получение запросов утверждения запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-105">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ba1c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ba1c-106">Permissions</span></span>
<span data-ttu-id="2ba1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2ba1c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ba1c-109">Permission type</span></span>      | <span data-ttu-id="2ba1c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ba1c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ba1c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ba1c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ba1c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ba1c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ba1c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ba1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ba1c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-114">Not supported.</span></span>    |
|<span data-ttu-id="2ba1c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ba1c-115">Application</span></span> | <span data-ttu-id="2ba1c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ba1c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ba1c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="2ba1c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ba1c-118">Request headers</span></span>
| <span data-ttu-id="2ba1c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ba1c-119">Name</span></span>       | <span data-ttu-id="2ba1c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba1c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ba1c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ba1c-121">Authorization</span></span>  | <span data-ttu-id="2ba1c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ba1c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ba1c-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2ba1c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba1c-125">Response</span></span>

<span data-ttu-id="2ba1c-126">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-126">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="2ba1c-127">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2ba1c-128">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="2ba1c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2ba1c-129">Example</span></span>
<span data-ttu-id="2ba1c-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ba1c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ba1c-131">Request</span></span>
<span data-ttu-id="2ba1c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ba1c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ba1c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```
# <a name="c"></a>[<span data-ttu-id="2ba1c-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ba1c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedapproval-myrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ba1c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ba1c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedapproval-myrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ba1c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ba1c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedapproval-myrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2ba1c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba1c-137">Response</span></span>
<span data-ttu-id="2ba1c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ba1c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
