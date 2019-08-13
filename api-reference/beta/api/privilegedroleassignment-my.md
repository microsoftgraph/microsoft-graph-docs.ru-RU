---
title: 'Привилежедролеассигнмент: My'
description: Получение привилегированных назначений ролей запрашивающей стороны.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5d7527106f0bb0a296a0abf8c20e99465d09653e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361053"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="9a029-103">Привилежедролеассигнмент: My</span><span class="sxs-lookup"><span data-stu-id="9a029-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a029-104">Получение привилегированных назначений ролей запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="9a029-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a029-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a029-105">Permissions</span></span>
<span data-ttu-id="9a029-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a029-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a029-108">Permission type</span></span>      | <span data-ttu-id="9a029-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a029-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a029-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a029-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a029-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a029-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a029-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a029-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a029-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a029-113">Not supported.</span></span>    |
|<span data-ttu-id="9a029-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a029-114">Application</span></span> | <span data-ttu-id="9a029-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a029-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a029-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a029-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="9a029-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a029-117">Request headers</span></span>
| <span data-ttu-id="9a029-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9a029-118">Name</span></span>       | <span data-ttu-id="9a029-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9a029-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a029-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a029-120">Authorization</span></span>  | <span data-ttu-id="9a029-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a029-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a029-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a029-123">Request body</span></span>
<span data-ttu-id="9a029-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a029-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a029-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a029-125">Response</span></span>

<span data-ttu-id="9a029-126">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a029-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a029-127">Пример</span><span class="sxs-lookup"><span data-stu-id="9a029-127">Example</span></span>
<span data-ttu-id="9a029-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9a029-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a029-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a029-129">Request</span></span>
<span data-ttu-id="9a029-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a029-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a029-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a029-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a029-132">C#</span><span class="sxs-lookup"><span data-stu-id="9a029-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a029-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a029-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a029-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9a029-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a029-135">Java</span><span class="sxs-lookup"><span data-stu-id="9a029-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-my-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9a029-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a029-136">Response</span></span>
<span data-ttu-id="9a029-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a029-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
