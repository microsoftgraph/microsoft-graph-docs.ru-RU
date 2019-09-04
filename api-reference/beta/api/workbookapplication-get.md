---
title: Получение Воркбукаппликатион
description: Получение свойств и связей объекта Воркбукаппликатион.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 00f8bf3b596aa1a4e58beb340fef6e2c94e834e3
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724003"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="8b2cf-103">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="8b2cf-103">Get workbookApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b2cf-104">Получение свойств и связей объекта Воркбукаппликатион.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-104">Retrieve the properties and relationships of workbookApplication object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b2cf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b2cf-105">Permissions</span></span>
<span data-ttu-id="8b2cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b2cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b2cf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b2cf-108">Permission type</span></span>      | <span data-ttu-id="8b2cf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b2cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b2cf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b2cf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b2cf-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-111">Not supported.</span></span>    |
|<span data-ttu-id="8b2cf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b2cf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b2cf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-113">Not supported.</span></span>    |
|<span data-ttu-id="8b2cf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b2cf-114">Application</span></span> | <span data-ttu-id="8b2cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b2cf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b2cf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b2cf-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b2cf-117">Optional query parameters</span></span>
<span data-ttu-id="8b2cf-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b2cf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b2cf-119">Request headers</span></span>
| <span data-ttu-id="8b2cf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8b2cf-120">Name</span></span>      |<span data-ttu-id="8b2cf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8b2cf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b2cf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b2cf-122">Authorization</span></span>  | <span data-ttu-id="8b2cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b2cf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b2cf-125">Request body</span></span>
<span data-ttu-id="8b2cf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b2cf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b2cf-127">Response</span></span>

<span data-ttu-id="8b2cf-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукаппликатион](../resources/workbookapplication.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-128">If successful, this method returns a `200 OK` response code and [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b2cf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8b2cf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b2cf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b2cf-130">Request</span></span>
<span data-ttu-id="8b2cf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8b2cf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b2cf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8b2cf-133">C#</span><span class="sxs-lookup"><span data-stu-id="8b2cf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b2cf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b2cf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8b2cf-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8b2cf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b2cf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b2cf-136">Response</span></span>
<span data-ttu-id="8b2cf-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b2cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
