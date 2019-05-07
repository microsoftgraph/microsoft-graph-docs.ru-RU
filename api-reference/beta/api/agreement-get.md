---
title: Получение соглашения
description: Получение свойств и связей объекта Agreement.
localization_priority: Normal
ms.openlocfilehash: a828e61420d744bbe63d10b9f5d8925a1355754a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636606"
---
# <a name="get-agreement"></a><span data-ttu-id="528b6-103">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="528b6-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="528b6-104">Получение свойств и связей объекта [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="528b6-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="528b6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="528b6-105">Permissions</span></span>
<span data-ttu-id="528b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="528b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="528b6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="528b6-108">Permission type</span></span>                        | <span data-ttu-id="528b6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="528b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="528b6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="528b6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="528b6-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="528b6-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="528b6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="528b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="528b6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="528b6-113">Not supported.</span></span> |
|<span data-ttu-id="528b6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="528b6-114">Application</span></span>                            | <span data-ttu-id="528b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="528b6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="528b6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="528b6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="528b6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="528b6-117">Request headers</span></span>
| <span data-ttu-id="528b6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="528b6-118">Name</span></span>         | <span data-ttu-id="528b6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="528b6-119">Type</span></span>        | <span data-ttu-id="528b6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="528b6-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="528b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="528b6-121">Authorization</span></span> | <span data-ttu-id="528b6-122">string</span><span class="sxs-lookup"><span data-stu-id="528b6-122">string</span></span> | <span data-ttu-id="528b6-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="528b6-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="528b6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="528b6-125">Request body</span></span>
<span data-ttu-id="528b6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="528b6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="528b6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="528b6-127">Response</span></span>
<span data-ttu-id="528b6-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="528b6-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="528b6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="528b6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="528b6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="528b6-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="528b6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="528b6-131">Response</span></span>
><span data-ttu-id="528b6-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="528b6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="528b6-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="528b6-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="528b6-135">Языках</span><span class="sxs-lookup"><span data-stu-id="528b6-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreement-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="528b6-136">Язык</span><span class="sxs-lookup"><span data-stu-id="528b6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreement-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
