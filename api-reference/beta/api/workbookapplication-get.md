---
title: Получение Воркбукаппликатион
description: Получение свойств и связей объекта Воркбукаппликатион.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5e2864a36db568184557340a44a5c447da44ec80
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451450"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="f851a-103">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="f851a-103">Get workbookApplication</span></span>

<span data-ttu-id="f851a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f851a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f851a-105">Получение свойств и связей объекта [воркбукаппликатион](../resources/workbookapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="f851a-105">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f851a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f851a-106">Permissions</span></span>
<span data-ttu-id="f851a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f851a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f851a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f851a-109">Permission type</span></span>      | <span data-ttu-id="f851a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f851a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f851a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f851a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f851a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f851a-112">Files.ReadWrite</span></span>     |
|<span data-ttu-id="f851a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f851a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f851a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f851a-114">Not supported.</span></span>    |
|<span data-ttu-id="f851a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f851a-115">Application</span></span> | <span data-ttu-id="f851a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f851a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f851a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f851a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f851a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f851a-118">Optional query parameters</span></span>
<span data-ttu-id="f851a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f851a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f851a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f851a-120">Request headers</span></span>
| <span data-ttu-id="f851a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f851a-121">Name</span></span>      |<span data-ttu-id="f851a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f851a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f851a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f851a-123">Authorization</span></span>  | <span data-ttu-id="f851a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f851a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f851a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f851a-126">Request body</span></span>
<span data-ttu-id="f851a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f851a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f851a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f851a-128">Response</span></span>

<span data-ttu-id="f851a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукаппликатион](../resources/workbookapplication.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f851a-129">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f851a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f851a-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="f851a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f851a-131">Request</span></span>
<span data-ttu-id="f851a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f851a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f851a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f851a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
# <a name="c"></a>[<span data-ttu-id="f851a-134">C#</span><span class="sxs-lookup"><span data-stu-id="f851a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f851a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f851a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f851a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f851a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f851a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f851a-137">Response</span></span>
<span data-ttu-id="f851a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f851a-138">Here is an example of the response.</span></span> 

><span data-ttu-id="f851a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f851a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
