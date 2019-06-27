---
title: 'Привилежедролеассигнмент: My'
description: Получение привилегированных назначений ролей запрашивающей стороны.
localization_priority: Normal
ms.openlocfilehash: 4d4b1c9df882c89ccd4b10d0dcaa904d060273fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264178"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="60ee1-103">Привилежедролеассигнмент: My</span><span class="sxs-lookup"><span data-stu-id="60ee1-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60ee1-104">Получение привилегированных назначений ролей запрашивающей стороны.</span><span class="sxs-lookup"><span data-stu-id="60ee1-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="60ee1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60ee1-105">Permissions</span></span>
<span data-ttu-id="60ee1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60ee1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60ee1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60ee1-108">Permission type</span></span>      | <span data-ttu-id="60ee1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60ee1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60ee1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60ee1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60ee1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60ee1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="60ee1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60ee1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60ee1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60ee1-113">Not supported.</span></span>    |
|<span data-ttu-id="60ee1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60ee1-114">Application</span></span> | <span data-ttu-id="60ee1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60ee1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60ee1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60ee1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="60ee1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60ee1-117">Request headers</span></span>
| <span data-ttu-id="60ee1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="60ee1-118">Name</span></span>       | <span data-ttu-id="60ee1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="60ee1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="60ee1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60ee1-120">Authorization</span></span>  | <span data-ttu-id="60ee1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60ee1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60ee1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="60ee1-123">Request body</span></span>
<span data-ttu-id="60ee1-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60ee1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60ee1-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="60ee1-125">Response</span></span>

<span data-ttu-id="60ee1-126">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект коллекции [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60ee1-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60ee1-127">Пример</span><span class="sxs-lookup"><span data-stu-id="60ee1-127">Example</span></span>
<span data-ttu-id="60ee1-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="60ee1-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="60ee1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="60ee1-129">Request</span></span>
<span data-ttu-id="60ee1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60ee1-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="60ee1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="60ee1-131">Response</span></span>
<span data-ttu-id="60ee1-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60ee1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="60ee1-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="60ee1-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="60ee1-136">C#</span><span class="sxs-lookup"><span data-stu-id="60ee1-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_my-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60ee1-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="60ee1-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_my-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="60ee1-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="60ee1-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_my-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignment-my.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-my.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-my.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
