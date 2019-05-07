---
title: Список соглашений
description: Получение списка объектов Agreement.
localization_priority: Normal
ms.openlocfilehash: 3d0594f37a3d88f7ff1ba9ea543e3b2d21ebc63a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636627"
---
# <a name="list-agreements"></a><span data-ttu-id="5f906-103">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="5f906-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f906-104">Получение списка объектов [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="5f906-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f906-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f906-105">Permissions</span></span>
<span data-ttu-id="5f906-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f906-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f906-108">Permission type</span></span>                        | <span data-ttu-id="5f906-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f906-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f906-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f906-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f906-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f906-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="5f906-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f906-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f906-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f906-113">Not supported.</span></span> |
|<span data-ttu-id="5f906-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f906-114">Application</span></span>                            | <span data-ttu-id="5f906-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f906-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f906-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f906-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="5f906-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f906-117">Request headers</span></span>
| <span data-ttu-id="5f906-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5f906-118">Name</span></span>         | <span data-ttu-id="5f906-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5f906-119">Type</span></span>        | <span data-ttu-id="5f906-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5f906-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5f906-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f906-121">Authorization</span></span> | <span data-ttu-id="5f906-122">string</span><span class="sxs-lookup"><span data-stu-id="5f906-122">string</span></span> | <span data-ttu-id="5f906-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f906-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f906-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f906-125">Request body</span></span>
<span data-ttu-id="5f906-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f906-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5f906-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5f906-127">Response</span></span>
<span data-ttu-id="5f906-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f906-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f906-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5f906-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f906-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f906-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="5f906-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f906-131">Response</span></span>
><span data-ttu-id="5f906-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f906-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5f906-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="5f906-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5f906-135">Языках</span><span class="sxs-lookup"><span data-stu-id="5f906-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreements-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f906-136">Язык</span><span class="sxs-lookup"><span data-stu-id="5f906-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreements-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
