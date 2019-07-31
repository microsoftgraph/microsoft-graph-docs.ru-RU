---
title: Получение Воркбукаппликатион
description: Получение свойств и связей объекта Воркбукаппликатион.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: b6f7e3a53f6d0210886afc8be3fc5c4e0cd87c15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995953"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="1a387-103">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="1a387-103">Get workbookApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a387-104">Получение свойств и связей объекта Воркбукаппликатион.</span><span class="sxs-lookup"><span data-stu-id="1a387-104">Retrieve the properties and relationships of workbookApplication object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a387-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a387-105">Permissions</span></span>
<span data-ttu-id="1a387-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a387-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a387-108">Permission type</span></span>      | <span data-ttu-id="1a387-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a387-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a387-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a387-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a387-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a387-111">Not supported.</span></span>    |
|<span data-ttu-id="1a387-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a387-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a387-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a387-113">Not supported.</span></span>    |
|<span data-ttu-id="1a387-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a387-114">Application</span></span> | <span data-ttu-id="1a387-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a387-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a387-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a387-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a387-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a387-117">Optional query parameters</span></span>
<span data-ttu-id="1a387-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1a387-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a387-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a387-119">Request headers</span></span>
| <span data-ttu-id="1a387-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1a387-120">Name</span></span>      |<span data-ttu-id="1a387-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1a387-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a387-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a387-122">Authorization</span></span>  | <span data-ttu-id="1a387-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a387-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a387-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a387-125">Request body</span></span>
<span data-ttu-id="1a387-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a387-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a387-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a387-127">Response</span></span>

<span data-ttu-id="1a387-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукаппликатион](../resources/workbookapplication.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a387-128">If successful, this method returns a `200 OK` response code and [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a387-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1a387-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a387-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a387-130">Request</span></span>
<span data-ttu-id="1a387-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a387-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a387-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a387-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a387-133">C#</span><span class="sxs-lookup"><span data-stu-id="1a387-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a387-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a387-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a387-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1a387-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1a387-136">Java</span><span class="sxs-lookup"><span data-stu-id="1a387-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a387-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a387-137">Response</span></span>
<span data-ttu-id="1a387-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a387-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
