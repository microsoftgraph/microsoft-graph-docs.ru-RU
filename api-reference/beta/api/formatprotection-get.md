---
title: Получение объекта FormatProtection
description: Получение свойств и связей объекта FormatProtection.
localization_priority: Normal
ms.openlocfilehash: 6e060e88944c069bd7399ab906f77fdfa6ccc405
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593587"
---
# <a name="get-formatprotection"></a><span data-ttu-id="be9b7-103">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="be9b7-103">Get FormatProtection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be9b7-104">Получение свойств и связей объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="be9b7-104">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be9b7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be9b7-105">Permissions</span></span>
<span data-ttu-id="be9b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be9b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be9b7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be9b7-108">Permission type</span></span>      | <span data-ttu-id="be9b7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be9b7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be9b7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be9b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be9b7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be9b7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be9b7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be9b7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be9b7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be9b7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be9b7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be9b7-114">Application</span></span> | <span data-ttu-id="be9b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be9b7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be9b7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be9b7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be9b7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be9b7-117">Optional query parameters</span></span>
<span data-ttu-id="be9b7-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be9b7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be9b7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be9b7-119">Request headers</span></span>
| <span data-ttu-id="be9b7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="be9b7-120">Name</span></span>      |<span data-ttu-id="be9b7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="be9b7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be9b7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be9b7-122">Authorization</span></span>  | <span data-ttu-id="be9b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be9b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be9b7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be9b7-125">Request body</span></span>
<span data-ttu-id="be9b7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be9b7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be9b7-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="be9b7-127">Response</span></span>

<span data-ttu-id="be9b7-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [FormatProtection](../resources/formatprotection.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be9b7-128">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be9b7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="be9b7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be9b7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="be9b7-130">Request</span></span>
<span data-ttu-id="be9b7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be9b7-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
##### <a name="response"></a><span data-ttu-id="be9b7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="be9b7-132">Response</span></span>
<span data-ttu-id="be9b7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be9b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="be9b7-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="be9b7-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="be9b7-137">Языках</span><span class="sxs-lookup"><span data-stu-id="be9b7-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_formatprotection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="be9b7-138">Язык</span><span class="sxs-lookup"><span data-stu-id="be9b7-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_formatprotection-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/formatprotection-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/formatprotection-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
