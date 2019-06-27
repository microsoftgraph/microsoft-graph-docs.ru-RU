---
title: Получение privilegedApproval
description: Получение свойств и связей объекта привилежедаппровал.
localization_priority: Normal
ms.openlocfilehash: 7a2f80dc001ea41c8446d84ff6a3310ebd7b3baf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268210"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="7d859-103">Получение privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="7d859-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d859-104">Получение свойств и связей объекта привилежедаппровал.</span><span class="sxs-lookup"><span data-stu-id="7d859-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d859-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d859-105">Permissions</span></span>
<span data-ttu-id="7d859-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7d859-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d859-108">Permission type</span></span>      | <span data-ttu-id="7d859-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d859-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d859-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d859-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d859-111">Привилежедакцесс. ReadWrite. AzureAD, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="7d859-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="7d859-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d859-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d859-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d859-113">Not supported.</span></span>    |
|<span data-ttu-id="7d859-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d859-114">Application</span></span> | <span data-ttu-id="7d859-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d859-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d859-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d859-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d859-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d859-117">Optional query parameters</span></span>
<span data-ttu-id="7d859-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d859-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d859-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d859-119">Request headers</span></span>
| <span data-ttu-id="7d859-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7d859-120">Name</span></span>      |<span data-ttu-id="7d859-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7d859-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d859-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d859-122">Authorization</span></span>  | <span data-ttu-id="7d859-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d859-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d859-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7d859-125">Request body</span></span>
<span data-ttu-id="7d859-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d859-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d859-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d859-127">Response</span></span>

<span data-ttu-id="7d859-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедаппровал](../resources/privilegedapproval.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d859-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="7d859-129">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="7d859-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7d859-130">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="7d859-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="7d859-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d859-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d859-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d859-132">Request</span></span>
<span data-ttu-id="7d859-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d859-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="7d859-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d859-134">Response</span></span>
<span data-ttu-id="7d859-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d859-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7d859-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="7d859-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7d859-139">C#</span><span class="sxs-lookup"><span data-stu-id="7d859-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d859-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d859-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7d859-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7d859-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_privilegedapproval-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
